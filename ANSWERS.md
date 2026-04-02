# Assignment Questions

## Instructions
Answer all 4 questions with detailed explanations. Each answer should be **3-5 sentences minimum** and demonstrate your understanding of the concepts.

---

## Question 1: Thread vs Process

**Question**: Explain the difference between a **thread** and a **process**. Why did we use threads in this assignment instead of creating separate processes?

A process, in my opinion, is a stand-alone program that runs independently and has its own memory and resources. In contrast, a thread is a smaller execution unit that shares memory and resources with a process. Threads are lighter and switch between them more quickly than processes, which are heavier and require more overhead to generate and manage. Because threads enable effective simulation of CPU scheduling, we employed them in this assignment rather than processes. Additionally, threads facilitate the sharing of data, including process information and the ready queue. Find out more about preventing race situations and thread synchronization.


---

## Question 2: Ready Queue Behavior

**Question**: In Round-Robin scheduling, what happens when a process doesn't finish within its time quantum? Explain using an example from your program output.
A process in Round-Robin scheduling is put back in the ready queue to wait for its next turn if it does not complete within its time quantum. This guarantees equity in all procedures.

This tendency is evident in the output of my software. For instance:
"P1 executing quantum [4000ms]"
"P1 completed quantum 4000ms │ Remaining time: 4954ms"
"P1 yields CPU for context switch"
"P1 (Priority: 5) added to ready queue"
This indicates that P1 was re-added to the ready queue since it failed to complete execution inside its time limit. It later reappears in the queue and is given another opportunity to run.

This cycle keeps on until the process is finished, which is displayed in the output later:
"P1 finished execution!"

This illustrates how Round-Robin scheduling equitably rotates processes, enabling each to run in brief bursts until it is finished.
[Paste a relevant snippet from your program output here showing a process being re-queued]
```

## Question 3: Thread States

**Question**: A thread can be in different states: **New**, **Runnable**, **Running**, **Waiting**, **Terminated**. Walk through these states for one process (P1) from your simulation.

## Question 3: Thread States

1. New:
P1 is in the New state when it is created in the program before execution begins. This happens when the Process object is instantiated.

2. Runnable:
P1 enters the Runnable state when it is added to the ready queue, as shown in the output:
"P1 (Priority: 5) added to ready queue"
At this stage, it is ready to be scheduled by the CPU.

3. Running:
P1 moves to the Running state when it starts executing on the CPU:
"P1 executing quantum [4000ms]"
This indicates that the thread is actively using CPU time.

4. Waiting:
After finishing its quantum but not completing execution, P1 gives up the CPU:
"P1 yields CPU for context switch"
Then it is placed again in the ready queue:
"P1 (Priority: 5) added to ready queue"
During this time, it waits for its next turn to run.

5. Terminated:
Finally, P1 reaches the Terminated state when it completes execution:
"P1 finished execution!"
At this point, its remaining time is 0 and it will not be scheduled again.

## Question 4: Real-World Applications

**Question**: Give **TWO** real-world examples where Round-Robin scheduling with threads would be useful. Explain why this scheduling algorithm works well for those scenarios.

### First Example: Web Server

An explanation:
A web server uses threads to manage several client requests at once.

Why Round-Robin is effective in this situation:
By ensuring that every request receives an equal amount of CPU time, Round-Robin keeps requests from starving.

--- ### Operating System Task Scheduling in Example 2

An explanation:
Operating systems oversee several concurrently running programs.

Why Round-Robin is effective in this situation:
By allocating equal time slots to each process, it ensures responsiveness and fairness.
 Synopsis

Important ideas I grasped from these questions:
1. Differences between threads and processes
2. Round Robin CPU Scheduling
3. The states and lifetime of threads

Ideas I should learn more about:
1. Synchronization of threads
2. Impasses
