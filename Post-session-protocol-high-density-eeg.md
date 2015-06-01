# Post Session Protocol High Density EEG
## On NetStation Mac
- Reminder: If you have not done so, save and close Net Station by pressing the **Close Session** button in the upper right hand corner of the NetStation window.  
- From the Net Station startup screen, go to **File > Open** to access archived sessions.  
  - Session files are usually located in: /Users/GilmoreLab/Documents/NetStation User Data/Sessions

  ![NS Open Archived Files](imgs/NS_Open_Archived_Files.jpg)  
  
  - to find the most recent session, click on the **Date** field in the Finder window. The small arrow should face downward to sort files in reverse date order (most recent first)  
  
  ![Take new Picture](imgs/NS_Open_Archived_Files.jpg)  

- From the **Tools** menu, open **Waveform Tools**  

![NS Open Waveform Tools](imgs/NS_Open_Waveform_Tools.jpg)  

- Run the Conatenate tool  
  - Press the **Add** button, and add the session file you wish to the Inputs window  
  - Select the **Concatenate Epochs for PowerDiva** tool from Specifications window  
    - To monitor progress, press the **Jobs/Results** button    
    - To run the tool, press the **Run** button  
    
![NS Concatenate Tool](imgs/NS_Concatenate_Tool.jpg)  

- Run the Export to Power Diva tool  

![NS Export_PowerDiva](imgs/NS_Export_PowerDiva.jpg)  

  - Add the **.cat** file you just created to the Inputs window by pressing the **Add** button  
  - Select the **Export for PowerDiva** tool from Specifications window   
    - To monitor progress, press the **Jobs/Results** button    
    - To run the tool, press the **Run** button  
      - This can take 3-8 minutes.  

- Quit Net Station  

- Quit the PowerDiva Video application on the PDvideo computer if you have not already done so.  

### Transfer data for analyses
#### Transfer to PDVideo
- On the NetStation computer desktop, double-click the **NetStation_Sessions@PDVideo alias** (highlighted in green)

![NS Sessions @ PDvideo alias](imgs/NS_@PDVideo.jpg)  

- Create a new folder with the participant ID (e.g. YYMMDDXXXX - test date (year, month, day) 4 digit participant ID #  
- Double click on **Sessions@Local** (highlighted in red). This opens a separate window to the local NetSataion Sessions folder.

![NS Sessions @ Local](imgs/NS_Sessions_Local.jpg)    

- Select the files for copy to the PDVideo machine (via the green folder)  
  -  Copy the following:  
    -  **original session file**  
    -  **raw data file** (.raw)  
    -  **cat data file** (.cat)  
    -  **gains file** (.GAIN)  
    -  **zero file** (.ZERO)  
    -  **impedance file** (.IMP)  
  - **Shift** or **command+Click** on these files and drag them to the green Net Station folder.  
    - This can take 5-10 minutes.  

![NS Transfer Files](imgs/NS_TransferedFiles.jpg)  
