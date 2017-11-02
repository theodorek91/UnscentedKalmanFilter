# Unscented Kalman Filter Project Starter Code
Self-Driving Car Engineer Nanodegree Program

In this project I was required to utilize an Unscented kalman filter to estimate the state of a moving object of interest with noisy lidar and radar measurements. Passing the project required obtaining RMSE values that were lower than the tolerance outlined in the project rubric.

The code is contained within the src folder.

main.cpp - is main program that comunicates with Simulator.
UKF.cpp contains code that runs tracking and calling of the Process and Update functions. 

Build folder holds build files created by cmake and make.

### Installation Notes

This repository includes two files that can be used to set up and install uWebSocketIO for either Linux or Mac systems. For windows you can use either Docker, VMware, or even Windows 10 Bash on Ubuntu to install uWebSocketIO. Please see this concept in the classroom for the required version and installation scripts.

Once the install for uWebSocketIO is complete, the main program can be built and run by doing the following from the project top directory.

mkdir build
cd build
cmake ..
make
./ExtendedKF

### Code Details

INPUT: values provided by the simulator to the c++ program

["sensor_measurement"] => the measurement that the simulator observed (either lidar or radar)

OUTPUT: values provided by the c++ program to the simulator

["estimate_x"] <= unscented kalman filter estimated position x ["estimate_y"] <= unscented kalman filter estimated position y ["rmse_x"] ["rmse_y"] ["rmse_vx"] ["rmse_vy"]

###Other Important Dependencies

cmake >= 3.5

make >= 4.1 (Linux, Mac), 3.81 (Windows)

gcc/g++ >= 5.4

### Basic Build Instructions

Clone this repo.
Make a build directory: mkdir build && cd build
Compile: cmake .. && make
On windows, you may need to run: cmake .. -G "Unix Makefiles" && make
Run it: ./ExtendedKF

### Project Instructions and Rubric

Note: regardless of the changes you make, your project must be buildable using cmake and make!

