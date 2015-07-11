# Setting up "password-free" log-ons to hammer

It can be incredibly convenient to log on to Unix based systems from the command line with minimal typing of passwords. The secure shell (*ssh*) protocol makes this possible. In the following, I describe how to set-up "password-free" command-line log-ons.

For every machine you want to enable "password-free" connections to (e.g., linux.imaging.psu.edu) you'll need to copy the public key to those machines (see steps 1.C onward).

## 1. From your local machine

I assume that you know how to open and use a terminal program on your local machine. Do that first.

### A. See if you have old references to hammer in your known_hosts file

`grep 'hammer' ~/.ssh/known_hosts`

If this returns lines that look like the following

`hammer.rcc.psu.edu ssh-rsa JDBKDS1239dks1ba300...` 

you will need to edit these lines from the file using the editor of your choice. Note that I have edited the text after the ssh-rsa part of the line for security reasons.  

It's wise to make a back-up of this file before you start editing it:

`cp ~/.ssh/known_hosts ~/.ssh/known_hosts_backup`

I like `nano` for this purpose, e.g.

`nano ~/.ssh/known_hosts`

Ctrl-K deletes lines, `Ctrl-X Y <return>` will save edits. 

Of course, use whatever editor you are comfortable using. Being a \*nix user is all about getting to choose which rope you like to hang yourself with.

### B. Generate new public key

`ssh-keygen -t rsa`

### C. Copy public key to home directory on hammer

`scp ~/.ssh/id_rsa.pub <your_psu_access_id>@hammer.rcc.psu.edu:~`

So, in my case, that would be 

`scp ~/.ssh/id_rsa.pub rog1@hammer.rcc.psu.edu:~`

We use the secure copy `scp` command that is based on `ssh` so that no one can grab our public key while it is in transit. 

### D. Log on to hammer

`ssh <your_psu_access_id>@hammer.rcc.psu.edu`

## 2. From your home directory on the hammer command line

### A. Make backup of authorized_keys file

`cd ~ # make sure you are in your home directory`
`cp ~/.ssh/authorized_keys ~/.ssh/authorized_keys_backup`

### B. Confirm that your public key is in your home directory

`ls | grep '~/id_rsa.pub'` from any directory, or just
`ls id_rsa.pub` from your home directory.

### C. Concatenate `cat` the public key to the `~/.ssh/authorized_keys` file

`cat ~/id_rsa.pub >> ~/.ssh/authorized_keys` from any directory or just
`cat id_rsa.pub >> ~/.ssh/authorized_keys` from your home directory.

### D. Logout

`logout`

## 3. From your local machine again

### A. Test password-free connection

`ssh hammer.rcc.psu.edu`

If this works, remove the public key from your home directory

`rm ~/id_rsa.pub`

# Make "aliases" for specific machines you connect to often

## 1. From your local machine

### A. Create or edit ~/.ssh/config
`nano ~/.ssh/config`

For each computer (host) you want to connect to, you need an entry like this:

    # hammer
     Host hammer
        HostName hammer.rcc.psu.edu
        User rog1

So, I have entries like this:

    # hammer
     Host hammer
        HostName hammer.rcc.psu.edu
        User rog1

    # linux.imaging.psu.edu
    Host hoth
        HostName linux.imaging.psu.edu
        User rog1

Change the User lines in the above to your own PSU access IDs unless you want your computer to think you are me.

### B. Test your new "alias"

`ssh hammer`

This should connect you to hammer without having to type `hammer.rcc.psu.edu`
