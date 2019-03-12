# Set up R and RStudio

## On PSU TLT's RStudio Server (recommended)

1. If on campus, make sure you are on the `psu` network. 
If you are off-campus, you must connect to PSU using a Virtual Private Network (VPN) client.
Cisco AnyConnect is the recommended VPN client.
If you do not have Cisco AnyConnect installed, visit <https://pennstate.service-now.com/sp?id=kb_article_view&sys_kb_id=ee330252db212788a318fb671d961981&sysparm_tsqueryId=5d397a69db1ea34497c9ffe61d961965&sysparm_rank=1> for installation instructions.
1. Log on to PSU TLT's RStudio server instance using your PSU access ID (e.g., `rog1` and password):

<https://lxclusterapps.tlt.psu.edu:8787/>

This gives you a full R and RStudio environment in a web browser.
You don't have to install R or RStudio.
You *do* have to install packages, however.

### Configure RStudio for `git` integration

1. From within RStudio, open the `Tools` menu and select the `Global Options...` item.
2. Select the `Git/SVN` panel in the left column. It is near the bottom of the list.
3. Check the `Enable version control interface for RStudio projects` checkbox at the top of the window.
4. Click on the `View public key` link to see if you have a valid SSH RSA Key already. 
5. If the window opens and contains a long text string that begins with "ssh-rsa" and ends with "<your_PSU_id>@lxclusterapps", where `<your_PSU_id>` is your PSU ID (e.g., `rog1`), you are half-way home.
6. If the window is opens and is empty, you must generate a new key:
    - ~~Close the window and click on the `Create RSA Key...` button.~~
    - From RStudio, select the `Terminal` pane. This will bring up a command line with a prompt that looks something like this: `bash-4.2$`.
    - Type `ssh-keygen.py` and hit return. This will generate an SSH key.
    - Type `ls ~/.ssh` and hit return. You should see something that looks like this:
```
bash-4.2$ ls ~/.ssh
id_rsa  id_rsa.pub  known_hosts
```
    - The `id_rsa.pub` is a file containing a 'public' key that you can save on GitHub so that GitHub knows who you are when you connect to it from the PSU TLT RStudio server.
    - (Optional) type `cat ~/.ssh/id_rsa.pub` to see the contents of this key file.
    - Select `Global Options...` from the RStudio `Tools` menu again.
    - Select `Git/SVN` from the left panel.
    - Select the `View public key` link to view the SSH key you just generated.
    - Copy the key to the clipboard (command+C on Mac)
8. Visit *your account* on GitHub. Rick's is at <https://github.com/rogilmore>.
9. Click on your avatar or photo in the upper right hand corner and select the `Settings` command.
10. From the list at left, select the `SSH and GPG keys` panel.
11. Look at the list of SSH keys.
12. If there are no SSH keys...
    - Press the `New SSH key` button.
    - Paste the key you generated in RStudio into the space provided.
    - Add a title like `PSU TLT` or `lxcluster`
    - Press the `Add SSH key` button to save the key.
13. If you see an existing key with `PSU TLT` or `lxcluster` you should already be ready to go.
14. Return to RStudio, hit `Apply` to save your changes, and `Ok` to exit the `Settings` panel.
15. Test the connection between RStudio and GitHub by cloning a repository.
    - Visit the lab protocols repository at <https://github.com/gilmore-lab/protocols>.
    - Click on the `Clone or download` button.
    - Confirm that the window title says `Clone with SSH`. If it does not, click on the `Use SSH` link on the upper right side.
    - Click on the clipboard icon to copy the `git@github.com...` link to the repository to your clipboard.
    - Switch back to RStudio.
    - Under the `File` menu, select the `New Project` option.
    - Select `Version Control`.
    - Select `Git` in the next window.
    - Paste the repository link you copies from GitHub into the `Repository URL` field.
    - Select a name for the local repository. I usually keep the name from GitHub, so in this case, I would use `protocols`.
    - Select a directory/folder where the repository will be copied to. I have an `rstudio/` folder I use for this. If you need to create a folder, you may do so.
    - Click on the `Create Project` button. This will copy the repository from GitHub to your personal (PASS) file space on PSU's servers. 