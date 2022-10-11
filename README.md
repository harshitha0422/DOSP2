# Project 2  Gossip Simulator
This is project 2 in the course COP5615 Distributed Operating System Principles. We implemented the gossip and push-sum algorithms over networks of arbitrary size with various network topologies.


##  Team Members
Harshitha Patel Velpula (UFID - 27659435)</br>
Vishesha Sadu (UFID - 29566305)
                       
## How To Run</br>
a. Compile all the erlang file and make sure beam files are available for each file.</br>
b. Execute the below command on the command line with the current directory set to the project to start the application.</br>
&emsp;  actor:run().</br>
c. Enter number of nodes when prompted</br>
d. Enter Topology when prompted</br> 
 &emsp;Options for Topology</br>
 &emsp;&emsp;1. line</br>
 &emsp;&emsp;2. full</br>
 &emsp;&emsp;3. 2D</br>
 &emsp;&emsp;4. Imp3D</br>
e. Enter the algorithm when prompted</br>
&emsp;Options for Algorithm</br>
 &emsp;&emsp;1. gossip</br>
 &emsp;&emsp;2. pushsum</br>



## Maximum Working Simulation
### What’s working?
As stated in the report, we created two distinct implementations for the gossip algorithm and one for push-sum. For all of the implementations, the line, complete, 2d, and imp3d topologies are functional.

### How many workers?
Depending on the topology, we have simulated different workers.</br>

### Largest Network for Gossip Algorithm:</br>
Full Topology - 2000 workers</br>
Line Topology - 1600 workers</br>
TwoD Topology - 1600 workers</br>
Imp3D Topology - 1600 workers</br>


### Largest Network for Push-Sum Algorithm:</br>
Full Topology - 4000 workers</br>
Line Topology - 500 workers</br>
TwoD Topology - 500 workers</br>
Imp3D Topology - 2000 workers</br>

Attached screenshots of highest actors we managed to deal with in each topology of both algorithms.

### Push Sum Algorithm:

<img width="917" alt="Screen Shot 2022-10-10 at 10 57 46 PM" src="https://user-images.githubusercontent.com/31062202/194990237-d98fa97f-a060-4611-829c-0e419c73d34a.png"></br>
Push Sum Algorithm – Full 4000N

<img width="782" alt="Line_500N" src="https://user-images.githubusercontent.com/31062202/194990263-e7277a47-5b8f-4b97-aa16-2d4c34e31462.png"></br>
Push Sum Algorithm – Line 500N

<img width="848" alt="Screen Shot 2022-10-10 at 9 45 27 PM" src="https://user-images.githubusercontent.com/31062202/194990332-293557f5-3704-4248-b99b-2c5c8694d4bf.png"></br>
Push Sum Algorithm – 2D 500N

![Uploading imp3d_pushsum_2000.png…]()</br>
Push Sum Algorithm – imp3D 2000N

### Gossip Algorithm:

![full_g_2000](https://user-images.githubusercontent.com/31062202/194990601-d01b6cd0-4d22-4164-89c0-dcb38e398a7f.png)</br>
Gossip Algorithm – Full 2000N

![line_g_1600](https://user-images.githubusercontent.com/31062202/194990496-45376084-488b-44c1-b9ba-09038de717dd.png)</br>
Gossip Algorithm – Line 1600N

![2d_g_1600](https://user-images.githubusercontent.com/31062202/194990508-59134c56-f63b-48e7-8ed6-d14d817d9279.png)</br>
Gossip Algorithm – 2D 1600N

![imp3d_g_2000](https://user-images.githubusercontent.com/31062202/194990556-ff7e5278-b6dc-4e21-8855-352766c45e9b.png)</br>
Gossip Algorithm – Imp3D 2000N![Uploading imp3d_g_2000.png…]()


















