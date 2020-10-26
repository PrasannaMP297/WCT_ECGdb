# Using Wilson Central Terminal ECG database clustering the patients data.
# t-SNE visualization. & implimentaion of DBScan on WCTECGdb
# Ackowladgement:

Moeinzadeh, H., & Gargiulo, G. (2019). Wilson Central Terminal ECG Database (version 1.0.1). 
PhysioNet. https://doi.org/10.13026/f73z-an96.


# Abstract:
The Wilson Central Terminal ECG Database (WCTECGdb) contains the Wilson Central Terminal (WCT), the voltage of right arm (RA), left arm (LA) and left leg (LL), six unipolar chest leads associated with three limb leads and six precordial leads.

With our ECG device, the potentials of RA, LA, LL and six true unipolar leads are measured using the right leg as the reference point. Having this configuration, we have been able to overcome the difficulty of recording the WCT in a clinical setting. Our data confirmed once again that the WCT does not have a small value, and could be as high as 241% of lead II and has standard ECG characteristics such as the p-wave and the t-wave. The dataset comprises of 540 ten-second segments recorded from 92 patients.

# Data Description:
The ECG signals were recorded from 92 patients (27 were female). Each recording is segmented to ten-second sections. As the total recording duration was different for each participant, the number of segments per patient ranges from one to thirty-one. The total number of ten-second segments is 540 for all patients. The average age of the patient population is 65.23 years (with a standard deviation of 12.12 years); the majority of the patients had a history of cardiac disease and had been admitted to the hospital.

We applied the low pass filter, and dc-removal filter to clean the dataset, and improve the signal to noise ratio. Both the raw and cleaned data are included in this dataset. The raw data is specified by -Raw in the signal names (e.g. V1-Raw). Each segment contains 37 signals listed below:

         * Raw
                    Three limb leads (I, II, III)
                    Six precordial leads (V1: V6)
                    Three limb potentials (LA, RA, LL)
                    Six true unipolar chest leads (UV1: UV6)  

         * Clean
                    Three limb leads (I, II, III)
                    Six precordial leads (V1: V6)
                    Three limb potentials (LA, RA, LL)
                    Six true unipolar chest leads (UV1: UV6) 
                    WCT
          
Dataset included age, gender, and patient diagnosis in the header file for each segment. system did not receive the patient diagnosis from the hospital for ten patients. Consequently, patient diagnosis is filled as "not reported"  for these patients.
