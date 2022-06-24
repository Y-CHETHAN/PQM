# Single server infinite capacity - Markovian Model

# Aim: 
To find 
      (a) average  number of materials in the system
      (b) average  number of materials in the conveyor
      (c) waitinging time of each material in the system
      (d) waitinging time of each material in the conveyor
if arrival rate of material  follows poisson process 4 per minuates and service rate of lathe machine follows exponential distribution with mean service rate 5 per minutes.


# Software required:  

Visual components and Python

# Theory:

  Queuing are the most frequently encountered problems in everyday life. For example, queue at a cafeteria, library, bank, etc. Common to all of these cases are the arrivals of objects requiring service and the attendant delays when the service mechanism is busy. Waiting lines cannot be eliminated completely, but suitable techniques can be used to reduce the waiting time of an object in the system. A long waiting line may result in loss of customers to an organization. Waiting time can be reduced by providing additional service facilities, but it may result in an increase in the idle time of the service mechanism. 

![image](https://user-images.githubusercontent.com/104613195/173292918-2583e4d3-a3d8-45fa-a577-9d0ebf79f0a5.png)

![image](https://user-images.githubusercontent.com/104613195/173292021-8c3b77dc-a9c2-4179-91ed-17e1db7039df.png)
 
# Procedure:
 
1. Calculate average number of materials to be waited in the conveyor using given data.
2. Create a empty project in visual component tool and add visual legacy component to the project.
3. Drag a feeder and place in a place and choose the appropriate material.
4. Calculate conveyor length using material size and average number of materials to be waited in the conveyor.
5. Choose the two conveyors from components,  add one conveyor with feeder.
6. Drag Lathe machine from machine library and place in the appropriate place.
7. Drag machine trending inlet and outlet from visual legacy and add them to the two conveyors in the appropriate manner.
8. Drag robot manager and robot from visual legacy and place in between two conveyors.
9. Connect all machine trending  inlet, outlet, robot manager and lathe machine using interface menu.
10. Run the program.

# Experiment:

![image](https://user-images.githubusercontent.com/104613195/175239086-d102fbc4-bc83-418d-8816-4c48fdbc9120.png)

# Program:

![image](https://user-images.githubusercontent.com/104613195/175240494-46c23d4d-ddc7-43ae-8fbc-c7da9edb2c83.png)

#  Output:

![image](https://user-images.githubusercontent.com/104613195/175240669-9eef6924-f33e-46f9-9c01-988b58480ce3.png)

# Result:
 
The average number of materials in the system is 4 and the conveyor is 3.2, and average waiting time of each materials in the system is 60 seconds and conveyor is 48 seconds are calculated.
