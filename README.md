# Flunnpy
Flunnpy is a project which aims to train an artificial neural network with CFD-(computational fluid dynamics)-data. For the first stept this ann should be able to predict the flow around a random geometry with same boundary condition. Ideas and approach are inspired by some projects:

https://github.com/loliverhennigh/Steady-State-Flow-With-Neural-Nets

https://medium.com/@jannik.zuern/neural-networks-for-steady-state-fluid-flow-prediction-part-1-856ef056da54

# Intention:
Why am I doing this? I am quite interested in neural networks and the capabilities of current AI development. As far as I know are ann quite good at detecting patterns. 
Furthermore I like simulations and especially CFD simulations. If well done they can save a lot of time during devolpement process, but proper setup of the problem can be tricky. In addition to this do simulations need some high level hardware for more complex problems. This often means that simulations are used when the first design phase is done and the milk is spilt. 
So why not trying to find patterns in the results of CFD simulations and train an ann to do the simulation for similar problems? It could support a developer in the early stages of design.

# Approach
First of all the scripts are written in python mostly. Prototyping is done using jupyter notebooks and only working scripts are transferred to .py scripts.  I will try to comment the code to keep it readable.
####Labeled data
Regarding the need of testing data the first step is to generate random geometries for the fluid dynamics simulation. For the simulation OpenFOAM is used. This is an open source simulation software for various numerical problems. Using snappyHexMesh as a meshing tools it is capable of scripted batch simulations for varied geometries. 
Creating the geometries and saving them in a format which can be read by the meshing tool (.stl) is done in the CreateSTL python file. 

This CreateSTL.py script is called by the Script "Run Cavity"

#### Run Cavity



# Model

#### Input

#### Boundary
![geometry /mesh](https://github.com/FredS1000/Flunnpy/blob/master/Pics/No34_A_0-0007_L0-1143_cavity_vel_1_Mesh.png)
#### Labeled data (fluid velocity in x and y direction) 
![velocity field x-direction](https://github.com/FredS1000/Flunnpy/blob/master/Pics/No34_A_0-0007_L0-1143_cavity_vel_1_X.png)

![velocity field y-direction](https://github.com/FredS1000/Flunnpy/blob/master/Pics/No34_A_0-0007_L0-1143_cavity_vel_1_Y.png)

#### First results
 ![First Results](https://github.com/FredS1000/Flunnpy/blob/master/Pics/Resultplot.png)
