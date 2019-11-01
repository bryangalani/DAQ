# DAQ
Data Acquisition using National Instruments DAQ.

We used a DAQ NI USB-6002 data acquisition system, which is a low-cost DAQ USB Device, manufactured by National Instruments. The equipment is used to store and process data acquired by, a current transducer and a voltage transducer using labVIEW.

The given file must be opened in LabVIEW. This files were programmed to use 2 pins as input data, that will be triggered by another pin in falling or rising edge (one file for each kind). All values will be saved in a .csv file (The address must be set by the user).

To open the .vi files, you need to use LabVIEW software (we used version 2018), combined with the NIDaq mx module to use the data Acquisition functions.

When oppening one of the files in LabView it will show this setup for you:

![LabVIEW file Setup](/Images/LabView01.png)

The left side is the graph which will plot the values of the input pins (2 pins = 2 line plots). The right side is the configuration of the DAQ by itself.

![LabVIEW file Setup](/Images/LabView02.png)

# Configuration
* The First purple box linked to AI Voltage, is responsible for setting the input pins, in this case, **AI6** and **AI7**.
* The orange box is the clock value (5000).
* The second purple box linked to Start Digital Edge is responsible for setting the trigger pin, in this case, **P1.1 / PF1**.
* The blue box linked to Start Digital Edge is responsible for setting the trigger edge (Falling or Rising), in this case, **Falling Edge**.
* The blue box linked to Analog 1D Wfm Nchan NSamp is responsible for the frame rate that will be plotted in the graph and logged in the file.
* Waveform Graph is the graph on the left side.
* Write to Measurement File box is responsible for recording the acquired data in a file, in this case, .csv file. Double click this box to change file path and format.
* The gray box around these boxes is a while loop.

**Take a look to the manual attached to see the pinout of DAQ**
