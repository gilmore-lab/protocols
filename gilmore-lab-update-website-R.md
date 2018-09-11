# Gilmore Lab Website Update Procedure - R

author: Andrea R. Seisler, ars17psu@gmail.com
date: 2017-02-25

## Required Software

R version 3.3.2 (2016-10-31)
R Studio Version 1.0.136 (2016-12-21)
GitHub syncing capabilities

## Background

- Website is hosted using GitHub pages.
- URL is <http://gilmore-lab.github.io>
- Site pages are created using R and Markdown.
- Version control uses git and GitHub.
- The site uses two GitHub repos:
    + <http://github.com/gilmore-lab/gilmore-lab.github.io>
        * Web site HTML, CSS, image and related files
        * Markdown and support files
        
## Editing/updating

- Open Sites
- Pull First




- Edit/add Markdown documents in gilmore-lab.github.io
	+ update .Rmd files
	+ knit HTML after every change
	+ save the files


- Build Website


- Commit all .Rmd and .html files

- Push Files


## To Do

- Update theme??
- User firefox to link local account and web

## Note
If you have trouble push the files, 
  "error: The requested URL returned error: 403 Forbidden while accessing https://github.com/gilmore-lab/gilmore-lab.github.io.git/info/refs
  fatal: HTTP request failed"
try this code in the shell:
git config remote.origin.url git@github.com:gilmore-lab/child-motion-psychophysics.git
git pull -u origin master
git push -u origin master