# Gilmore Lab Projects  
small change

## EEG Projects
- update protocols
  - Calibrate-Monitor.md
  - Post-session-protocol-high-density-eeg.md
  - ssvep-high-density-setup.md
  - mofo-3-pattern-psychophysics **completed**
  
 
## MOFO Child Tuning
### Goal
Collect data from 25 participants
### Participants
- 10 previous Participants  
- 27 additional participants  
- all demographic data is located on databrary: https://nyu.databrary.org/volume/144
- Discarded Data
  - Too Few Blocks (1)
  - Channels Over Threshold (2)
  - Refusal to Wear Net (1)
  - Experimenter Error (3)
   

### Data Processing
- 10 participants reprocessed with PD Video  
  - Raw Threshold Detector = 60 / Blink Threshold = 60  
  - Raw Threshold Detector = 100 / Blink Threshold = 100 
- additional participants processed with PD Video using two threshold detector settings
  - Raw Threshold Detector = 60 / Blink Threshold = 60
  - Raw Threshold Detector = 100 / Blink Threshold = 100  

### To Do
- **Completed** Reprocess the 10 previous participants at the settings Raw Threshold Detector = 100 / Blink Threshold = 100
  - *Difficulty: After copying the data from Box to the PowerBook G4, no files are showing up in PD Video, just directories. However everything shows up in the Finder Window.*
     - raw data was copied from data collection computers and completely reprocessed.  

- **Completed** Create R script to prepare output files from PD Video for the analysis script pipeline - R script converted from moco  
  
- **Completed**R script (mofo-RLS-file-convert.R) will run in individual folders  

  - Sample code:
    - setwd("/Users/ars17/Box Sync/b-gilmore-lab-group Shared/gilmore-lab/projects/optic-flow/optic-flow-eeg/mofo/mofo-child-tuning/sessions/060310lesu/ThreshBlink100")
    - source('~/Desktop/Rscript/mofo-RLS-file-convert.R')
    - mofo.RLS.file.convert()  

- fix R script to run as a function through all datasets in the sessions folder
   

  
## MOCO INF_2Pat_LamRad
### Goal
- Collect data from 25 participants
### Participants
- 5 Participants
- all demographic data is located on databrary: https://nyu.databrary.org/volume/146
- Discarded Data
  - Too Few Blocks ()
  - Channels Over Threshold (2)
  - Refusal to Wear Net (2)
  - Experimenter Error (4)
  - no RLS file created (1) - rerun this dataset through processing!

### Data Processing
- 5 participants processed with PD Video  
  - Raw Threshold Detector = 200 / Blink Threshold = 200  



## Symm Sorting Task
### Goal
- Collect Data from 20 participants
- Process, Analyze data along with 11 datasets collected previously 
- Submit to: XXXXX

### Participants
- 22 additional participants
- demographic data located on psubrainlab google drive: My Drive/participants/symm-session-log
  - This does not include the 11 datasets collected previously 
- Total participants: 33   

- *Where are the demographic data for the 11 previous datasets located?*

### Data Processing
- R script is being created by Michelle and Rick

### To Do
- Process data after R script is created
- Put demographic data on databrary - create new volume
- what are the questions in the exit interview used for?

## MOCO Psychophysics
### Goal
- Collect data from 25 4-8 year old Child participants  

### Paradigm Status
- Instructions located  on Github repo: moco-3-pattern-psychophysics
  - How to run an experiment: moco-3-pattern-psychophysics-experiment-instructions.md **complete**
  - How to alter, generate and run an experiment: moco-3-pattern-psychophysics-checklist.md **complete**


### To Do
- purchase a game controller: http://www.walmart.com/ip/29016209 **complete**
- pilot with kids
- Determine parking procedure for Moore. 


## Status of lab computers  
- The computers that were taken off the network cannot be put back on the network  

### Gilmorelab01  

#### Hardware    
- iMac(21.5-in, Late 2009)
- 3.06 GHz Intel Core 2 Duo
- 8 GB 1067 NGz DDR3
- ATI Radeon HD 4670 256 MB  
- 2TB SATA Disk
 
#### Software  
- OS X Yosemite version 10.10
- Box Sync
- datavyu (1.3.4)
- Dr. Cleaner - gilmorelab appstore
- Final Cut Pro (10.2.2) - gilmorelab appstore
- GitHub Desktop
- Git
- Google Chrome
- Matlab R2014b w/ Psychtoolbox
- Microsoft Office
- Mou (2014)
- Quicktime Player - gilmorelab appstore
- R (3.2.1)
- R Studio (0.99.489)
- Skype
- Sublime (2.0.2)
- Xcode - gilmorelab appstore
- Zotero  

#### To Do
- Clean install of OS
- Set up wireless network
- reinstall software listed above

### Gilmorelab02  

#### Hardware  
- iMac(21.5-in, Late 2009)
- 3.06 GHz Intel Core 2 Duo
- 8 GB 1067 NGz DDR3
- ATI Radeon HD 4670 256 MB 
- 1TB   

#### Software   
- OS X Yosemite version 10.10
- Box Sync
- datavyu (1.3.4)
- GitHub Desktop
- Git
- Google Chrome
- Microsoft Office
- Mou (2014)
- Quicktime Player - gilmorelab appstore
- R (3.2.1)
- R Studio (0.99.489)
- Skype
- Zotero

#### To Do
- Clean install of OS
- Set up wireless network
- reinstall software listed above


### 27in iMac

#### Hardware  
- iMac(27-in, Mid 2011)
- 2.7 GHz Intel Core i5
- 4 GB 1333 MHz DDR3
- AMD Radeon HD 6770 512 MB   
- 1TB SATA hard drive

#### Software   
- OS X Yosemite version 10.10.5
- Box Sync ?
- datavyu (1.3.4)
- Fetch
- GitHub Desktop ?
- Git ?
- Google Chrome
- Microsoft Office
- Mou (2014)
- Quicktime Player
- R (3.2.1)
- R Studio (0.99.489)
- Skype 
- Zotero

#### To Do
- Problem: Memory usage is currently 60% with no applications running
  - Solution: Beef up RAM- Order 1: [(4GBx2) DDR3 1333 MT/s](http://www.amazon.com/Crucial-PC3-10600-204-Pin-CT2K4G3S1339M-Notebook/dp/B008LTBIT4/ref=sr_1_1?s=pc&ie=UTF8&qid=1449252336&sr=1-1&keywords=PC3-10600+%281333%29+DDR3+204-pin+SO-DIMM#Ask) from Amazon - completed
- Install new RAM - completed 2/3/2016
- After memory upgraded
  - Install Box Sync
  - Install Git
  - python/web items
  - 1 password
  


## Mt. Nittany IRB Application   
### Application
- Completed application located: Box Sync ▸ b-gilmore-lab-group Shared ▸ gilmore-lab ▸ irb ▸ protocols ▸ active ▸ MtNittanyRecruiting  
  
### To Do   
- Please review (Rick)   

## Video Coding 
### Coding for Indiana/India data
- All files are located on ars17psu google drive 
  - 'Andrea-Everything you need to start working' slides
     - updated to include correct server address
  - Participant information: Locomotion_codinglog2015

- Complete coding for a few participants
- Train students to complete coding - started on 1/15/2016

- Problem: Error connecting to server using instructions on slide 6 - connect to mac slide 3/5 (12/4/2015)
- An email was sent to Swapnaa (12/4/2015) to check that I have the correct server address.
- Received correct server address (12/16/2015). I am ready to go.
- Students completing video tutorial then everyone is coding the same dataset. 
- After coding the same dataset is complere, I want to look similarities and differences between coders.

- Datavyu scripts
  - script to make sure all codes are lowercase
  - template .opf file
  - complete reliability coding for 20% of participants (entire dataset)
    - copy coding column with blank codes have a different coder complete this
  - put all coded data back on the server
  - 

### Keep Datavyu notes
- keep notes of things that work well or don't work well while coding Indiana/India data
