## Simulation and tuning of parameters

In **datagenerator.py**, different tracks can be drawn for testing - linear, circular, racing. Their shape can be adjusted in their corresponding functions.

In **codegenerator.py**, the actual generation of the code takes place. The model, cost function and constraints are specified here. Also all the settings of the solver can be chosen here.

In **simulator.py**, all the code needed for interaction with the generated code is here, the most important function is `solve` inside which different situations can be tested. For example, the initial position of the vehicle can be set, some noise can be added to the measurements, etc.

In **parameters.py**, all the parameters of the vehicle and of the solver are set and called from here.

From **visualisator.py**, different functions can be used to show and analyse the results of a simulation. It also contains code to plot and compare from a file in which the values are saved (in testing.py).

Everything is run from **testing.py**, starting from generation of the code, generation of the track and ending with visualisation of the results (histogram of solve times and plotted track).
