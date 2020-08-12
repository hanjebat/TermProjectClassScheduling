# Group Members
Assmida Binti Hassdee (1819114) <br>
Ayza-Adani Binti Jaffry (1813100) <br>
Hannah Binti Huda (1814022)

# Introduction

CPU Scheduling is a process determining which process will execute first while another process is on hold or in waiting state due to insufficient of CPU resources. The aim of CPU scheduling is to make the system faster and efficient. This project focused on non-preemptive scheduling. In non-preemptive scheduling method, the CPU has been allocated to a specific process. 

# Consideration

There are several types of scheduling algorithms: First Come First Serve (FCFS), Shortest-Job-First (SJF), Shortest Remaining Time, Priority Scheduling, Round Robin Scheduling and multilevel scheduling. For this project we have considered First Come First Serve(FCFS), Shortest Job First(SJF) and Priority Scheduling. We applied processes with same data (arrival time, burst time and priority) using FCFS, SJF and priority scheduling to analyze the average time taken and average turn around time.

# Analysis
Input for the project consists of three processess.

Process 1: 2201 <br>
Duration: 3 <br>
Priority: 2 <br>
Arrival Time: 1 <br>
<br>
Process 1: 3401 <br>
Duration: 2 <br>
Priority: 3 <br>
Arrival Time: 2 <br>
<br>
Process 1: 1103 <br>
Duration: 1 <br>
Priority: 1 <br>
Arrival Time: 3 <br>


## FCFS
In first come first serve schedulling algorithm, the process which arrives first, gets executed first. 

### Output <br>
Order in which processes gets executed: 1103 -> 2201 -> 3401 <br>
Average waiting time = 2.66667 <br>
Average turn around time = 4.66667

## SJF
In shortest job first algorithm, the scheduler selects process to work based on the burst time. In non-preemptive shortest job first algorithm, the burst time of the processes should be known to the processor in advance. <br>
### Output <br>
Order in which processes gets executed: 2201 -> 1103 -> 3401<br>
Average waiting time = 1.33333 <br>
Average turn around time = 3.33333

## Priority Scheduling
In priority scheduling, the scheduler selects process to work based on the priority lists. Priority scheduling algorithm is suitable for a real-time operating system. In non-preemptive priority scheduling algorithm, if a new process with higher priority than current running process appear in ready queue, the new process will be positioned at the head of ready queue and the process will be execute immediately. If there are processses with the same priority, it will be executed based on FCFS algorithm.<br>
### Output <br>
Order in which processes gets executed: 1103 -> 2201 -> 3401 <br>
Average waiting time = 1.66667 <br>
Average turn around time = 3.66667 <br>

# Conclusion
The calculation of three algorithms shows different average waiting time. SJF has the shortest average waiting time compared to FCFS and priority scheduling. 
