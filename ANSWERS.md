# Assignment Questions

## Instructions
Answer all 4 questions with detailed explanations. Each answer should be **3-5 sentences minimum** and demonstrate your understanding of the concepts.

---

## Question 1: Thread vs Process

**Question**: Explain the difference between a **thread** and a **process**. Why did we use threads in this assignment instead of creating separate processes?

**Your Answer:A process is an independent program with its own memory space, resources, and execution environment. A thread, however, is a lightweight unit of execution that runs inside a process and shares the same memory with other threads. Threads need far fewer resources to create and switch between than processes. This makes them faster and more efficient for simulations. In this assignment, we used threads because we needed multiple “processes” to run at the same time while sharing data structures like the ready queue and process map. Using real OS processes would have added extra overhead and complexity. In contrast, threads let us simulate CPU scheduling behavior accurately and efficiently.**

[Write your answer here. Consider: What is a process? What is a thread? How do they differ in terms of memory, resources, creation overhead? Why are threads more suitable for this simulation?]

---

## Question 2: Ready Queue Behavior

**Question**: In Round-Robin scheduling, what happens when a process doesn't finish within its time quantum? Explain using an example from your program output.

**Your Answer:In Round‑Robin scheduling, if a process does not finish within its assigned time quantum, it is interrupted and placed back into the ready queue to wait for another turn. This ensures fairness by giving every process equal CPU time in cycles. The process will run again only after all other processes in the queue have had their turn.**

[Write your answer here. Describe the specific behavior - where does the process go? When does it run again? Give an example from your actual program output showing a process that was re-queued.]

Example from my output:
```**
? P5 completed quantum 4000ms │ Overall progress: 40%
   Remaining time: 5976ms
? P5 yields CPU for context switch

? P5 added to ready queue │ Burst time: 9976ms │ Priority: 4
**
[Paste a relevant snippet from your program output here showing a process being re-queued]
```

**Explanation of example:**
**
In this snippet, P5 used up its entire 4000ms quantum but still had 5976ms of burst time remaining. Because it did not finish, the scheduler forced it to yield the CPU and placed it back into the ready queue. P5 will wait behind the other processes and eventually receive another quantum later in the cycle. This behavior demonstrates the fairness and cyclic nature of Round‑Robin scheduling.**
[Explain what's happening in the output snippet you pasted]

---

## Question 3: Thread States

**Question**: A thread can be in different states: **New**, **Runnable**, **Running**, **Waiting**, **Terminated**. Walk through these states for one process (P1) from your simulation.

**Your Answer:**
[Write your answer here. For each state, explain when P1 enters that state during the simulation. Use your understanding of the code to trace through the lifecycle.]

1. **New**: [When is P1 in New state?]**P1 is in the New state immediately after its thread object is created but before it starts running.**

2. **Runnable**: [When does P1 become Runnable?]**When P1 is added to the ready queue at the beginning of the simulation, it becomes Runnable because it is ready to run but not yet executing.**

3. **Running**: [When is P1 Running?]**P1 enters the Running state when the scheduler selects it and calls currentThread.start(). In your output, this happens when P1 executes its full quantum of 3182ms.**

4. **Waiting**: [When/why would P1 be Waiting?]**P1 would enter a Waiting state if it were blocked or waiting for I/O, but in this simulation, the main waiting behavior is simulated by re‑queuing. Since P1 finishes in one quantum, it does not re‑enter the queue or wait again.**

5. **Terminated**: [When is P1 Terminated?]**After P1 completes its entire burst time (3182ms) and prints “P1 finished execution!”, it enters the Terminated state. At this point, the thread has completed its run method and will not be scheduled again.**

---

## Question 4: Real-World Applications

**Question**: Give **TWO** real-world examples where Round-Robin scheduling with threads would be useful. Explain why this scheduling algorithm works well for those scenarios.

**Your Answer:**

### Example 1: Operating System Task ** Scheduling[Name of application/scenario]

**Description**: 
**Operating systems run small tasks at the same time. These tasks include background services updates to the user interface and user applications.**
[Describe the real-world scenario or application]

**Why Round-Robin works well here**:
**Round-Robin helps to make sure every task gets some CPU time. This prevents one task from freezing the system. It makes sure everything is fair and response times are good. This is very important when many tasks are running at the time.**
[Explain why Round-Robin scheduling is suitable. Consider fairness, responsiveness, predictability, etc.]

### Example 2:Multiplayer Online Games** [Name of application/scenario]

**Description**: 
**Games handle things at once. These things include player actions, physics updates and network events.**
[Describe the real-world scenario or application]

**Why Round-Robin works well here**: 
**Round-Robin helps to make sure each players action is handled properly. No one player or event can use all the CPU time. This keeps the game smooth and responsive, for all players**
[Explain why Round-Robin scheduling is suitable. Consider fairness, responsiveness, predictability, etc.]

---

## Summary

**Key concepts I understood through these questions:**
**1. So what is the difference between threads and processes. The main thing to know is that threads are more efficient than processes. This is because threads are lighter and they use memory than processes. The difference between threads and processes is very important to understand.
2. Now let us talk about Round‑Robin scheduling. This is a way to schedule processes. When a process is running it gets an amount of time this is called a quantum. If the process is still running when this time is up then Round‑Robin scheduling will stop it. Put it at the end of the line. This is called re-queuing. The process will have to wait until it's its turn again to run.
3. A thread has a lifecycle. This means it is born it. It dies. The lifecycle of a thread is important to understand. A thread can be, in states. It can be. It can be waiting. The thread will move between these states during its lifecycle. The lifecycle of a thread is very important to know when working with threads**

**Concepts I need to study more:**
**1. I want to make sure everything happens at the time without any issues. This means avoiding problems that can occur when multiple things are happening simultaneously like data getting messed up. Synchronization helps with that
2. We also need to look into ways to schedule tasks and manage multiple things happening at once. This includes controlling how they all work together at the time, which is really important, for making sure everything runs smoothly and efficiently.**
