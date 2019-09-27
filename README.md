# DAQ
Data Acquisition using National Instruments DAQ

We used a DAQ NI USB-6002 data acquisition system, which is a low-cost DAQ USB Device, manufactured by National Instruments. The equipment is used to store and process data acquired by, a current transducer and a voltage transducer using labVIEW.

The given file must be opened in LabVIEW and is programmed to use 2 pins as input data, that will be triggered by another pin in falling or rising edge (one file for each kind). All values will be saved in a .csv file (The address must be set by the user).

To open the .vi files, you need to use LabVIEW software (we used version 2018), combined with the NIDaq mx module to use the data Acquisition functions.
