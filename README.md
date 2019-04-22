# ANN-MPC

**ANN-MPC** is a public repository of codes and datasets a new control scheme for a two-level converter based on combining Model Predictive Control (MPC) with feed-forward Artificial Neural Network (ANN), with the aim of getting lower THD and improving the steady and dynamic performance of the system for different types of loads. 

The proposed ANN-based control strategy undergoes two main steps: 
1. the use of MPC, as an expert or a teacher, for generating the data required for training off-line the proposed neural network using standard supervised learning, under full-state observation of the system; 
2. once the off-line training is performed, the trained ANN can successfully control the output voltage of the inverter, without the need of using MPC at test time, as illustrated in the following figure.
![Screenshot](ANN-MPCDiagram.pdf)
