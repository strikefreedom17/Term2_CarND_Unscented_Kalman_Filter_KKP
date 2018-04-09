# Term2_CarND_Unscented_Kalman_Filter_KKP

[image1]: ./UKF_Dataset1.png
[image2]: ./UKF_Dataset2.png


In this project, an Unscented Kalman Filter (UKF) technique is utilized to estimate the state of a moving object given the noisy lidar and radar measurements. The spec for the root mean square error (rmse) of all 4 states [px, py, vx, vy] is given by [.09, .10, .40, .30] for Dataset 1. The UKF is implemented in c++. The details of UKF algorithm are given in the src folder:

Given the two datasets, the rmse values are:

Dataset 1: RMSE = [0.0691, 0.0830, 0.3333, 0.2343] <  [.09, .10, .40, .30 (RMSE spec)], and

Dataset 2: RMSE = [0.0685, 0.0693, 0.5846, 0.2473].

The simulation results are shown as following:
![UKF estimation result given Dataset 1, Green: Estimated states, Red: Lidar measurement, Blue: Radar measurement][image1] 


![UKF estimation result given Dataset 2][image2] 

To starting code for this project is given by (https://github.com/udacity/CarND-Unscented-Kalman-Filter-Project).
The Simulator used in this project can be downloaded [here](https://github.com/udacity/self-driving-car-sim/releases). 
To test the script from the project top directory, please follow these steps:

1. mkdir build
2. cd build
3. cmake ..
4. make
5. ./UnscentedKF


## Other Important Dependencies

* cmake >= 3.5
  * All OSes: [click here for installation instructions](https://cmake.org/install/)
* make >= 4.1 (Linux, Mac), 3.81 (Windows)
  * Linux: make is installed by default on most Linux distros
  * Mac: [install Xcode command line tools to get make](https://developer.apple.com/xcode/features/)
  * Windows: [Click here for installation instructions](http://gnuwin32.sourceforge.net/packages/make.htm)
* gcc/g++ >= 5.4
  * Linux: gcc / g++ is installed by default on most Linux distros
  * Mac: same deal as make - [install Xcode command line tools](https://developer.apple.com/xcode/features/)
  * Windows: recommend using [MinGW](http://www.mingw.org/)
