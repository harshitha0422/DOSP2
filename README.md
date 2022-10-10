# Project 2  Gossip Simulator
In this project we have implemented a distributed gossip simulator using Erlang. 

##  Team Members
Harshitha Patel Velpula (UFID - 27659435)</br>
Vishesha Sadu (UFID - 29566305)
                       
## How To Run</br>
a. Compile all the erlang file and make sure beam files are available for each file.</br>
b. Execute the below command on the command line with the current directory set to the project to start the application.</br>
&emsp;  actor:start().</br>
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
Depending on the topology, we have simulated as many as 4098,4192 workers.


## Simulations and Result
The program has been executed for workers scaling in the powers of 2 from 8 to 4096. The statistics: wall clock was used to record the time. You can refer to the data.xlsx for more information. We can infer from the graph plotted for each topology for the gossip algorithm, from all the simulations gives us the information that the gossip algorithm the line performs badly whereas 2D topology and Imp2D topology behaves similarly until 2K workers, then they diverge in elapsed time. The same is observed in Push Sum Algorithm Imp2D and 2D diverge after the same 2K workers, unlike former algorithm observation, here Imp2D is performing slightly better than 2D topology as per Table 1,2. So we have inferred the results from the data being visualized into graphs. 

In Push Sum Algorithm, the line topology start performing well after hitting the 3.5K workers count, and in case Gossip algorithm the full topology keeps up with Imp2D and 2D. But both full and Imp2D continue to behave same way until 2.5K workers whereas the 2D continued a good perform after 2K workers previously mentioned. As all of these results help us understand the pushsum unique round based logic Is</br>
So, each of topology are as implemented as follows:</br>

__Full Network__ is such a way that every actor is a neighbor of all other actors. As in every actor will talk directly to any other actor.</br>

__2D Grid__ is such way that all actors form a 2 dimensional grid, such as a way actors can only talk to its adjacent neighbors</br>

__Line topology__ is such as a way that actors are arranged in a line, such that all actor has only 2 neighbors (one left and one right unless except for the first and last actor).</br>

__Imperfect 2D Grid__ arrangement is that one random other neighbor is selected from the list of all actors (8+1 neighbors).
The criterion for convergence is that we have a tracker function that should receive confirmation from all workers that they received the rumor so that we can declare conversed fully.</br>

Figure 1: Gossip Algorithm Simulations


Figure 2: PushSum Algorithm Simulations
Table 1: Gossip Algorithm
Table 2: Push Sum Algorithm
 
Push Sum Algorithm – Full 4096N


Push Sum Algorithm – Line 4096N





Push Sum Algorithm – Imp2D 4096N


Push Sum Algorithm – 2D 4192N





Gossip Algorithm – Full 4096N



Gossip Algorithm – Line 4096N




Gossip Algorithm – Imp2D 4096N


Gossip Algorithm – 2D4192N





