# Video Coding Manual for Locomotion Coding Study  

## How to video code   
1.  Make sure you’re using a keyboard that has a dedicated keypad
2.  Go to [Locomotion_codinglog2015](https://docs.google.com/spreadsheets/d/1zxMLBf0ayY_wHaJLWKZRl28KQyDpNmKFHhMfYwMYqtA/edit#gid=1826061711), WhereWeAt_INDIA tab  
3.  Choose subjects labeled “pick me”
4.  Make a new folder for subject in **looxcie/1B_LooxcieIndia/04_annotation/04_Locomotion/1_Datavyu_Loco/**
5.  Open Datavyu* (ideally version 1.2), click add data button
6.  Go to **looxcie/1B_LooxcieIndia/01_videos_AllMasters/** and find the corresponding subject folder that contains all clips 
7.  If the clip has a version named “_**withrotation**”, code that version (and not the original version)!
  * cloumn name = loco
  * code name = locomotion
8.  Use the template ‘loco_template.opf’
  * Add new column, name it **loco** (pay attention to this case :))
9.  In the controller window, make sure the red triangle is dragged to the very beginning (0:00.00)
10.  Click “Add new cell”, time stamp 0:00.00 should come up in cell box
  * if text = "cell1" rename it to "locomotion"  
11.  Code for stationary “s”, movement “m” - ALWAYS lower case
12.  Some videos might display the words “do no code”. Code those portions as “_”
13.  Some portions of videos are hard to view (too dark, too blurry, etc) - code those portions also as “_”
14.  Press 0 on keypad to create new cell and set previous offset
15. Be sure that there is end time stamp when you are finished coding video (press Set End Cell to ensure this, or “.” or “9” on the keypad)
16.  Save under the subject’s folder in **looxcie/1B_LooxcieIndia/04_annotation/04_Locomotion/1_Datavyu_Loco/[your participant folder] → Clip name: ex. 008AP_01”**
17.  Export file (File > Export File >) under **looxcie/1B_LooxcieIndia/04_annotation/04_Locomotion/1_Datavyu_Loco/ → Clip name: ex. 008AP_01”**







## How to complete reliability coding


#### After a dataset is fully coded a script called ‘MakeReliabilityColumn.rb’ will be run. This script is located in the ‘India_Videos’ folder. This will generate the following in each coded .opf file:
  * a new column called ‘rel_loco’
  * every 5th cell from the ‘loco’ column will be copied to this new column
  * This column will have the onset time included, but the offset time and code (m,s,_) will have to be coded.
  * Run the script by: MakeReliabilityColumn.rb is a batch script that will run through all .opf files in the ~/India_Videos/ folder (this will be run by ARS after all ‘loco’ column coding is complete.
  * A coder that did not code the ‘loco’ column will have to code the ‘rel_loco’ column.
  * Hide the ‘loco’ column when coding the ‘rel_loco’ column.
  * Highlight the column to be hidden
  * Spreadsheet > Hide Selected Columns

## Examples of timing moving and stationary 



### Timing  
- 2 seconds of no movement will be considered stationary

### Examples of moving 
- The infant must be moving through space. Essentially this means that the trunk of the baby is moving.  
- flipping a baby from back to stomach  
- lifting an infant  
- putting an infant down  

### Examples of stationary  
- baby rolling around  
- baby being slightly swayed 

### FAQS
**Infant on back lifted and flipped to belly. does this count as movement?**   
- Yes!  
**Mom picks kid up and sways ever so gently, slightly, that the view doesn't change much. Is this Stationary?**    
- Yes!  
**Baby sat on a park swing and swinging wildly. Is this movement?**    
- Yes!  
**If the adult is holding the child while bending over to pick something up is that moving or stationary?**  
- s (before bending) 
- m (while bending, > 2 seconds) OR s (while bending, < 2 seconds)  
**If the adult is holding the child and sits down then stands up quickly is that moving or stationary?**
- If the motion of standing or sitting takes more than 2 sec code as movement, if it takes < 2 sec code as stationary.
**What should i do if an infant is put in the car and the car is moving? I counted that as movement since they're going somewhere, but I wasn't sure how to count stopping at stoplights and all that since the infant is facing the seat and there's not a clear view of the outside. Or, since the baby's view isn't changing really, does it count as stationary?**
- If there's a change in state for more than 2 seconds (like if they're stopped at a light for 1 minute) then that's stationary for the duration of time they're at the light.








