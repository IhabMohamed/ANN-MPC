# ANN-MPC

**ANN-MPC** is a public repository of codes and datasets of a new control scheme for a two-level converter based on combining Model Predictive Control (MPC) with feed-forward Artificial Neural Network (ANN), with the aim of getting lower THD and improving the steady and dynamic performance of the system for different types of loads. 

The proposed ANN-based control strategy undergoes two main steps: 
1. The use of MPC, as an expert or a teacher, for generating the data required for training off-line the proposed neural network using standard supervised learning, under full-state observation of the system. Here is the MPC model used for generating the training data [MPC-3-Phase-Inverters](https://github.com/IhabMohamed/MPC-3-Phase-Inverters).  
2. Once the off-line training is performed, the trained ANN can successfully control the output voltage of the inverter, without the need of using MPC at test time, as illustrated in the following figure.

![ANN-MPCDiagram](ANN-MPC/Dataset/TrainingDiagram.png)

#### Citing

If you use the ANN-MPC or dataset in an academic context, please cite the following publication:

Paper: [A Neural-Network-Based Model Predictive Control
of Three-Phase Inverter With an Output LC Filter](https://ieeexplore.ieee.org/abstract/document/8819887)

```
@article{mohamed2019neural,
  title={A Neural-Network-Based Model Predictive Control of Three-Phase Inverter With an Output LC Filter},
  author={Mohamed, Ihab S and Rovetta, Stefano and Diab, Ahmed A Zaki and Do, Ton Duc},
  journal={IEEE Access},
  year={2019}
}
```
