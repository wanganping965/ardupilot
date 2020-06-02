This is a example MATLAB multicopter backend for the JSON SITL interface. Its mostly physics based, Copter.m is used to setup the property's of the vehicle. This does some basic performance plots of motor thrust and power from the given motor and propeller parameters. The vehicle parameters are then saved in a .mat file, Hexsoon.mat in this case as the model is roughly based on the Hexsoon EDU450. This file is then loaded into SIM_multicopter.m and the connection to SITL started. SIM_multicopter is written in such a way that it should be simple to save a set of parameters for another vehicle type, such as a hexacopter and run them with the same model.

There are many simplifications in the model, the most egregious of which is a arbitrary thrust multiplier to get a sensible hover thrust from the correct vehicle parameters.