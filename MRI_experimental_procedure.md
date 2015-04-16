# MRI Experimental Procedure Protocol
## Recruiting
- Adults are typically recruited from the [Psychology Department Subject Pool](https://pennstate.sona-systems.com)

## Pre-Session
- Arrive 15 minutes prior to the study time.
- Organize Consent (2 copies), [MRI screening form] (https://www.imaging.psu.edu/sites/sleic/files/3T_screening_safety_form_061911.pdf), vision screening form.

## Participant Arrival
- Greet and welcome participant in room 6 Chandlee

## Informed Consent and MRI screening
- Explain testing procedures throughly, answer questions thoughtfully.
- Have participant sign and initial 2 copies of the informed consent.
- The person obtaining consent must sign both copies of the informed consent.
- One copy of the consent is for the participant and one is for the lab records.
- Have the participant complete the MRI screening form.
- Screen participants for eligibility; if ineligible, be sensitive and polite.
- Explain the task

## Vision screening
- Complete vision screening if participant does NOT self report 20/20 vision.
- Follow the instrucations located in 'MR Vision Screen Protocol.docx'.
- Complete Vision screening that is on the door to room 7C. 
- Choose appropriate lenses based on the chart on the side of the participant lockers.
- Goggles and lenses are located in the top drawer of the file cabinet with the printer on it in room 7.
- Complete the ‘MRI Vision Screen Data Sheet.docx’

## Participant ID
- Tell the MR Technologist the participant ID.
  - Test Date, Test Time, sub, participant number
  - Format: yyyy-mm-dd-hhmm-sub-xxxx
  - e.g. 2015-04-05-1130-sub-5000

## Testing Preparation - prior to participant entering the room
- Ensure that the 20 Channel Head Coil is being used.
- Open the following on the desktop:
  - Matlab R2011b
  - Pictures (Start > Documents > Libraries > Pictures > Sample Pictures)
  - The Calibration Screen (image_calibration)
  - A notepad document (New Text Document)
- Test the Grips 
  - Ensure the Text Document screen is active
  - Test the trigger grip in notepad (see table below)
  - Close the Text Document

Finger | Output
------ | ------
Left Thumb | a
Left Index | b
Right Thumb | c
Right Index | d

- Check the Projector Calibration Screen
  - Ensure the Calibration screen is active and full screen
    - press the button in the bottom middle of the calibration screen window to make it full screen
    - press Esc to exit full screen
  - Check the calibration screen image for focus and clarity prior to the participant entering the scanner room

## Participant Preparation
- Have the participant empty their pockets, remove all jewelry, metal, belts, phone, etc. and place in a locker.
- MR Technologist duties
  - Review the MRI screening form with the participant.
  - Escort the participant into the scanner room, have them lie on the bed, and scoot up into the head coil.
  - Tape the emergency squeeze ball to their shirt.
  - Set the 0 location on the participant
  - Have the participant enter the scanner bore.
  - Ensure the participant can see all columns and rows of the calibration screen
    - The calibration screen exits out of full screen after a short time. Make sure it is full screen when the participant 
  - Ensure the participant's comfort and safety.
- Researcher duties
  - Hand the participant the trigger grip for the dominant hand.
  - Briefly explain the task again

## Testing
- Close Calibration Screen
- Run Picture Slideshow during Localizer and MPRage
  - Location: Documents > Pictures
  - Choose 'Slide Show' at the top of the window.
  - Press 'Esc' to exit
- Run Matlab Script on Projector PC
  - This script is run 3 times - once for each EPI scan
  - Script: SLEIC-Projects>rog1>wallpaper_groups_event_related_fmri>code>Symmetry-2>symmetry.m
  - Open Matlab (R2011b)
  - Change directory to: SLEIC_Projects\rog1\wallpaper-groups-event-related-fmri\code
\Symmetry-2
  - At the Matlab prompt (>>) type 'symmetry'
  - Press 'Enter' to Run
    - Session Information
      - Subject ID: This is generated in the format of yyyymmddThhmmss
      - Number of runs: 1
      - Presentation Interval: 1.2
      - TR: 2.5
      - Trigger: yes
  - Press Confirm
  - Press Yes
  - Press Space
    - Screen will say "waiting for trigger"
  - Ask Debra to start EPI scan

Note: Press Esc to stop stimuli

## Post-Session
- Thank participant
  - Record participation credit on Sona Systems or complete payment form.
- Record session information in ‘MRI-Session Log’ on Gilmore-lab google drive. 
- Copy first and last page of consent form.
- Make sure the MRI technologist has the screening form and the copy of the consent form. 
- Have the MRI Technologist transfer MRI data in the ‘nifti’ format to Hoth: /nfs/imaging-data/3Tusers/rog1/symm
- Save Matlab data located at (SLEIC-Projects>rog1>wallpaper_groups_event_related_fmri>code>Symmetry-2>Data>yyyymmddThhmmss) to External Drive.

## Post-Processing/Analysis
- rsync MRI data from Hoth to Hammer
  - rsync automatically runs once per week on Saturday 
- Save Matlab data from External Drive to /gpfs/group/sleic/rog1/symm/projects/fmri/event-related-fmri-pilot/behavioral/"participant-folder"/"matlab-folders"

- Perform Timing Correction First prior to any other processing steps.


  
