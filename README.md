# Flunnpy
Flunnpy is a project which aims to train an artificial neuronal network with CFD-(computational fluid dynamics)-data. For the first stept this ann should be able to predict the flow around a random geometry with same boundary condition. Ideas and approach are inspired by some projects:

https://github.com/loliverhennigh/Steady-State-Flow-With-Neural-Nets

https://medium.com/@jannik.zuern/neural-networks-for-steady-state-fluid-flow-prediction-part-1-856ef056da54

# Intention:
Why am I doing this? I am quite interested in neuronal networks and the capabilities of current AI development. As far as I know are ann quite good at detecting patterns. 
Furthermore I like simulations and especially CFD simulations. If well done they can save a lot of time during devolpement, but proper setup of the problem can be tricky. In addition to this do simulations need some high level hardware for more complex problems. This often means that simulations are used when the first design phase is done and the milk is spilt.  
So why not trying to find patterns in the results of 

# Approach
Regarding the need of testing data the first step is to generate random geometries for the fluid dynamics simulation. For the simulation OpenFOAM is used. This is an open source simulation software for various numerical problems. Using snappyHexMesh as a meshing tools it is capable of scripted batch simulations for 
This is done in the CreateSTL python file. 

The secon
