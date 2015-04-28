# High-Density VEP Set-Up Checklist

## MONITOR
- Turn on the **CRT monitor** on the cart in 120G

## AMPLIFIER

- In 120G Chandlee remove cables from amplifier and connect them to pegs on wall.
 
<IMG SRC="/imgs/rear-of-amplifier.pictClipping.jpg" align="middle" ALT="Rear of NetAmps 200">

- Wheel amp between the monitor and the subject chair so that it is to the right of the subject chair. 
  **ALWAYS PULL AMP BACKWARDS TO PREVENT TIPPING**

- Plug the 4 cords from the wall ports connecting rooms G and H into respective ports (Digital input, USB, and TTL input external timebase) of the amplifier. 
- Turn power on (I = on).

![Rear of NetAmps 200 Data Cables](imgs/rear-of-amplifier-data-cables.pictClipping.jpg)

- Turn small switch on amplifier to **NORMAL**
  - If this is on another setting during calibration and impedance check, you will see an error stating that everything is out of specification. 
  - If there is an error, you must begin the setup from step one again.

 
## COMPUTERS

- In 120H Switch on power of large surge protector on bottom left shelf.

- Switch on power of smaller, thin surge protector on second shelf (ignore lights; always on).

- Turn on **PD Video** and **NetStation** computers, and both monitors.

  - If either monitor screen is unresponsive, you may need to toggle to the correct computer via the gray KVM switches on the top left (PD Video / Link 15) and right (NetStation  / PD Host) shelf.

- Turn on external timebase, behind the monitors (switch is back, right side).

- Remove the plug from the external timebase outlet labeled **OUT**. (Clock Out stays in).
 
![Rear of External Timebase](imgs/rear-of-ext-timebase.pictClipping.jpg)

- Make sure that white round switch on top of the left KVM switch is set to B.

<IMG SRC="/imgs/White-Switch.jpg" ALT="White Switch on top of Black KVM Switch" align="absmiddle">

- On PD Video computer, open Power Diva Video 3.4 software. (icon label says alias)

![Power Diva Video icon](imgs/power-diva-video-icon.pictClipping.jpg)
 
- In Power Diva Video, go to Configuration > Video Manager. In **Mode** window, make sure the calibrated video setting is selected: 

	- 800 x 600, 72 Hz, 8 bit
 
 ![Power Diva Video Manager](imgs/2015-04-28-calibration.jpg)

### Prepare Stimuli

#### For Child and Adult
- In Run mode (pull-down tab), choose **Auto Sequence**. 
- In Msg mode (pull-down tab), choose **Net Station**.
- In Stim Set, Go to Open, and choose the appropriate stimulus set.
  - Child
    - 
  - Adult

<IMG SRC="/imgs/RunModeAutoRun.jpg" ALT="Open Stimulus Set - Auto Sequence" align="absmiddle" width="50%">

#### For Infant
- In Run mode (pull-down tab), choose **Baby Mode**. 
- In Msg mode (pull-down tab), choose **Net Station**.
- In Stim Set, Go to Open, and choose the appropriate stimulus set.
  - inf_2pat_lamrad (most used)
  - inf_2pat_lamrot
  - inf_2pat_radrot

<IMG SRC="/imgs/RunModeBabyMode.jpg" ALT="Open Stimulus Set - Baby Mode" align="absmiddle" width="50%">

- Press the Run button. In the DAQ Rate Settings window, there is a binary code to confirm. On the side of the external time box facing you, there are silver switches (up = 1, down = 0). Read the binary code in the PD Video window from right to left, and check to make sure that the switches on the timing box correspond to this code. If they don't match, notify the PI. If they do, press Cancel.

![Determine Time Base Code](imgs/power-diva-autorun.pictClipping.jpg)

### Prepare Net Station

- Go to the Net Station computer and log in with the **gilmorelab** account (w/ lab password - **0baby0**).
	
- In the dock at the bottom of the screen, click on the icon for Net Station (purple icon) to open the program.
 
![NetStation icon](imgs/start-netstation.pictClipping.jpg)

- When the window pops up, there should be a key symbol with the words **Wenger** on the bottom left-hand side. If it is not there, this means that the NS HASP key is not plugged in.

- In the Net Station window, click **New Session**
- Select the session template labeled **Power Diva Adult Set Up**.
	 

## AFTER PARTICIPANT ARRIVES

- Enter participant ID, Experiment Name, Date of birth, and net serial number. Lab uses the following standard ID number for each session: YYMMDD_ID# (Test Date_Participant ID number).

![Enter participant session info](imgs/ns-enter-session-info.pictClipping.jpg)

- **Begin Session**.

- Run Zeros and Gains (should run automatically).

![Gains](imgs/Gains.jpg)

![Zeros](imgs/Zeros.jpg)

- Place the net on the EEG Participant

- After netting, plug the net into the articulating arm.

![Connect arm to amp](imgs/Net-plugged-into-articulating-arm.jpg)

- Measure Impedance.
  - Go to the **Panels** menu at the top of the screen and select **Impedance**
  - Then click the **Measure Impedance** button.
  - Adjust channels as necessary. 
  - Click **Save & Close** when satisfactory.

![Measure Impedance](imgs/measure-impedance-window.pictClipping.jpg)

- Go to the **Panels** menu at the top of the screen and select **Dense Waveform Display**.

![Dense waveform](imgs/dense-waveform-display.pictClipping.jpg)

- Turn small switch on amplifier to **EXTERNAL TIMEBASE**.

![External Time Base](imgs/external-timebase-switch-on-amp.pictClipping.jpg)

## Experimental Setup

- The monitor should be located 60cm from the bridge of the nose on the participant
- The chair height should be set so the participant is looking directly at the **X** in the middle of the screen.
- High Density
  - Baby Mode (Researcher in the room)
    - Record: Use the Keyboard to record (**R**) 
      - When recording there is an **X** in the middle of the screen.
    - Pause Study: Use the keyboard to pause (**W**)
      - When paused there is an **X** with a **circle** around it in the midde of the screen
    - Use the toys to keep attention toward the monitor
  - Auto Sequence
    - Pause Study: The keyboard **space bar** in the testing chamber or on the PD Video computer
    - Continue Study: The **Continue** button must be clicked in the Power Diva software
- Low Density
  -  Game controller is used to record and pause

## Run Experiment

- In Power Diva Video, press the **Run** button in the **Stim Set** window
- The **Auto Run Settings** window will open
- **Check the box** in the Net Station Recording control window labeled **Start/Continue Net Station Recording**
- Press **Run**.

![Run Session](imgs/AutoRunSettings_NS Box Checked.jpg)

- Try to get the following number of blocks of data:
  - Infant: 6
  - Child: 10
  - Adult: 12
  
- On the Net Station computer, make sure the “Recording” symbol is displayed on the upper left-hand side of the screen. Also, make sure the event flag labeled “DIN4” is present, as well as a flag below this with the condition number (e.g., “c004”).
  - the flag "p003" means that the study was paused

![NS Recording Symbol](imgs/NS-Recording-Screenshot.jpg)

## AFTER SESSION

- Once recording is complete, select the **close session** button on the Net Station computer (this saves the session).

- Return computers and other devices to their default settings.

- Return and replug amplifier to its default setup.

- Clean net and begin [data export](ssvep-data-export.md) (separate protocols).

