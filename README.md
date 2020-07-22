# Square_trajectory_drone

This project is built on Flytos using flytsim and Gazebo for simulation of drone. 
This file contains step by step guide on how to run the sqr_traj_drone.py file.    
 Prerequisite:
 1. Flytos Installation : For installing flytos on your Ubuntu 16.04(used flavour of linux by me) you need an account of Flytbase and using following link you can install flytos in your system. Installing flytos will automatically install required ros version and gazebo simulator tool for this project.
 Link for flyos: https://docs.flytbase.com/flytos/getting-started/setup-flytos/odroid-xu4/installing-flytos-dependencies-in-your-custom-image
 2. Flytsim Installation : For installing flytsim from your flytbase account download the file from following link of flytbase docker engine. 
 link for flysim docker : https://github.com/flytbase/flytsim-docker/releases/tag/v0.2.3
 After that open the terminal, go to flytdocker directory, select your os and select your graphic card(in my case I used intelgraphics). 
 Then run command 'sudo ./setup.sh' to install docker engine and docker-compose in your system. 
 
 This will complete required steps to launch flytsim and gazebo for simulation.
 
 Creating project:
    To create sqr_traj_drone.py file I used Python api's from FlytAPI. 
 1. First we import required libraries and API from flyt_python. 
 2. Then instance of flyt navigation named as 'drone' was created.
 3. For taking value from user of sidelength of square Argument parser is used. 
 4. Using take_off, position_set and land trajectory of drone is defined. In take_off api height(>1.5m) is mentioned in the code.
 5. lastly we save this file in .py format.
 
 Launching project:
 1. For launching the FLytsim on top of gazebo we have to open intelgraphics file from flytdocker in terminal.
 2. Then run command 'sudo ./start.sh' to launch flysim on top of Gazebo. You will see gazebo environment with Drone at rest.
 3. To run our file first we need to launch openshell in flysim. For that run command 'sudo ./openshell.sh' .
 4. Then in openshell, run your code by executing command 'python /"flie location"/"file name"' . 
 This will start simulation in Gazebo environment.

    © 2020 GitHub, Inc.
    Terms
    Privacy
    Security
    Status
    Help

    Contact GitHub
    Pricing
    API
    Training
    Blog
    About

