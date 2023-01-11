# Deep Learning in Scientific Computing
Deep learning project with the aim of studying the preliminary design of a thermal energy storage.
This repository contains the code for the project for the with the ETH course "Deep Learning in Scientific Computing", held by professor Siddhartha Mishra in Spring semester 2022. The aim of the project is studying the preliminary design of a thermal energy storage.
The main objective of the project is to apply machine learning algorithms to solve various tasks related to the preliminary design of a thermal energy storage.
The device is used in solar power plants to store thermal energy during the charging phase and release it for production of electricity during the discharging phase. The thermal energy is stored due to the interaction of a fluid and a solid phase. During the charging state the fluid is injected at high temperature from one end of the storage and heats the solid up. In contrast, during the discharging phase the reverse process occurs: cold fluid flows from the opposite end and absorbs heat from the solid. Between charging and discharging idle phases take place, where no fluid enters the thermal storage.
Therefore, at any instant of time the thermal storage can be in one of the following states:
1. Charging;
2. Idle between charging and discharging;
3. Discharging;
4. Idle between discharging and charging;
Together the four states establish a cycle and the same process is repeated for several cycles until the thermal storage reaches a periodic or stationary regime.


The project is developed into six different tasks:

## Task 1: Noisy Function Approximation
<img align="right" height="140" src="https://github.com/angelognazzo/Deep-Learning-Scientific-Computing/blob/main/Task1/figure%20submission/outputTf0task1.png"></img>
Given noisy measurements of the fluid and solid temperature, taken at the top end of the storage during the entire process, the goal is to approximate the maps that describes the evolution over time of the fluid and solid temperature.
<br/><br/>

## Task 2: Learning Observables in High Dimensional Space
<img align="right" height="110" src="https://github.com/angelognazzo/Deep-Learning-Scientific-Computing/blob/main/Task2/figure%20submission/outputtask2.png"></img>
In order to evaluate the performance of the storage, non-dimensional observables are usually defined. One of the is the capacity factor. 
The goal is to learn the map from a set of several input variables to the capacity factor.
<br/><br/>

## Task 3: Time Series Forecasting
<img align="right" height="140" src="https://github.com/angelognazzo/Deep-Learning-Scientific-Computing/blob/main/Task3/figure%20submission/outputTf0.png"></img>
Similarly to the first task the goal is to approximate the maps that describes the evolution over time of the fluid and solid temperature. 
Here the interestet is in the future (or out of samples) predictions of the fluid and solid temperature. In other words, the training data consists of time measurements t_i registered in a frame [0; T] and we want to forecast the fluid and solid temperature in the frame [T; Tend].
<br/><br/>

## Task 4: Inference of Fluid Velocity
<img align="right" height="120" src="https://github.com/angelognazzo/Deep-Learning-Scientific-Computing/blob/main/Task4/figure%20submission/output4c.png"></img>
Given noisy measurements of the fluid temperature, taken at the bottom end of the storage x = L during the charging phase of the first cycle, the goal is to infer the velocity of the fluid (using bayesian inference).
<br/><br/>

## Task 5: Design of Storage Geometry
<img align="right" height="140" src="https://github.com/angelognazzo/Deep-Learning-Scientific-Computing/blob/main/Task5/figure%20submission/outputtask5.png"></img>
In this task the interest is in the optimal design of the thermal storage. Formally, the aim of the task is to find the control parameters y = (D; v), with D in [2; 20] being the diameter of the storage and v in [50; 400] its volume, such that the capacity factor is exactly CF_ref = 0.45.
<br/><br/>

## Task 6: PINNs for solving PDEs
<img align="right" height="140" src="https://github.com/angelognazzo/Deep-Learning-Scientific-Computing/blob/main/Task6/figure%20submission/outputtask6.png"></img>
In this task the goal is solving the system of equations that describes the temperature evolution of the solid and fluid phases in the termal storage with
physics informed neural networks.


