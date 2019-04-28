# *Folders Description*
* `Dataset Folder`: contains the dataset and its description, which has been used for training and testing the proposed ANN-based control scheme. These data, which have been collected by [MPC](https://github.com/IhabMohamed/MPC-3-Phase-Inverters), comprises 70 samples, which are divided into 60 samples for specific resistive loads, whereas only 10 samples represent the case where the inverter is directly fed a non-linear load (i.e., diode-bridge rectifier). For each sample, the simulation is run, using [MPC](https://github.com/IhabMohamed/MPC-3-Phase-Inverters), under various operating conditions such as simulation time (i.e, number of output voltage cycles), sampling time $$T_s$$, filter capacitor C, filter inductance L, DC-link voltage Vdc, and reference voltage. More details about each sample are given in
[Dataset.pdf](Dataset/Dataset.pdf). 

* In [InputFeatures](Dataset/InputFeatures) Folder, we have stored all instances and its targets which is called by [prepareData_forANN.m](prepareData_forANN.m), in order to gether and convert these data in the proper form for training the proposed ANN using [ANN_training.m](ANN_training.m).    

