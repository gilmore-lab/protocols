# Gilmore Lab

## Power Diva 3.x Export

- Exp_MATL_HCN_128_Avg

	- AXX format (Spectral amplitude on X axis) suitable for Matlab

	- Creates .mat files by condition number Axx_c001.mat ... Axx_c000n.mat, plus Montage_ssn.mat

	- Each .mat file contains the following:

		- Amp, spectral amplitude nFr x nCh
		- Cos, "real" coefficient of DFT
		- Cov, inter-channel covariance?
		- DataUnitStr, data unit string, typically "microVolts"
		- Sin, "imaginary" coefficient of DFT
		- Wave, time domain nT x nCh
		- cndNmb, condition number, e.g., 1 if c001
		- dFHz, delta frequency in Hz (spectral width of DFT bin)
		- dTms, delta time (width of each time step)
		- i1F1, index of 1F1, starts at 0
		- i1F2, index of 1F2, starts at 0
		- nCh, number of channels, typically 128
		- nFr, number of frequencies, nFr X dFHz = maxFreq = NyquistF/4
		- nT, number of temporal samples nT x dTms = maxTrialTime
		- nTrl, number of trials

- CndParams_*

	- MOCO Paradigm

		- iSess	
		- iCond	
		- NTrials	
		- Eye	
		- DomNon	
		- CondNotes	
		- Treatment	
		- Level	
		- iPdm	
		- PdmVer	
		- ViewDist	
		- MeanLum	
		- SweepType	
		- Step	
		- Start	
		- End	
		- ModType	
		- ModInfoName	
		- ModInfo	
		- Density	
		- Glass Pat	
		- Glass Coher	
		- Pair Sep	
		- Glass Dir	
		- Glass Radial	
		- Field Diam	
		- Temp Freq1	
		- Contrast	
		- Pix Size HV1	
		- Dir Mean1	
		- Dir Range1	
		- Lifetime1	
		- Bidirectional1	
		- Radial1	
		- Mot Coher1	
		- FieldMask	
		- LoopType	
		- Temp Freq2	
		- Pix Size HV2	
		- Dir Mean2	
		- Dir Range2	
		- Lifetime2	
		- Bidirectional2	
		- Radial2	
		- Mot Coher2	
		- FK_Prc	
		- FK_Sess	
		- PK_Cond

- RLS.txt

	- iSess, YYYYMMDD_HHMM	
	- iCond, condition number
	- iTrial, trial index, typically 0 for non sweep	
	- iCh, channel index, hc001-Avg ... hc128-Avg 	
	- iFr, frequency index	
	- AF, actual frequency	
	- xF1, multiple of fundamental (F1)	
	- xF2, multiple of 2nd fundamental (F2)	
	- Harm, harmonic label, e.g., "1F1"	
	- FK_Cond, ?	
	- iBin, ?	
	- SweepVal, used for sweep	
	- Sr, "real" coefficient of DFT	
	- Si, "imaginary" coefficient of DFT	
	- N1r, left noise sideband real coefficient	
	- N1i, left noise sideband imaginary coefficient
	- N2r, right noise sideband real coefficient	
	- N2i, right noise sideband imaginary coefficient	
	- Signal, signal amplitude sqrt( Sr^2 + Si^2)	
	- Phase, phase of amplitude atan2( Si, Sr )	
	- Noise, noise amplitude	
	- StdErr, for computing T^2 Circ	
	- PVal, T^2 Circ value	
	- SNR	
	- LSB, Left significant bin, used in sweep mode
	- RSB, Right significant bin, used in sweep mode	
	- UserSc	
	- Thresh	
	- ThrBin	
	- Slope	
	- ThrInRange	
	- MaxSNR

- SsnHeader.txt

	- iSess	
	- SessDate	
	- Operator	
	- LastName	
	- FirstName	
	- BirthDate	
	- DueDate	
	- DayAge	
	- Sex	
	- Handedness	
	- DaqRateHz, Data Acquisition rate in Hz	
	- NChan, number of channels, typically 128
	- Montage, typically HCN_128	
	- Notes	
	- Treatment	
	- Level	
	- DomEye	
	- FK_Mtg	
	- PK_Sess