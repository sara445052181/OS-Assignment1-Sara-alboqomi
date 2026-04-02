# Assignment Questions

## Instructions
Answer all 4 questions with detailed explanations. Each answer should be **3-5 sentences minimum** and demonstrate your understanding of the concepts.

---

## Question 1: Thread vs Process

**Question**: Explain the difference between a **thread** and a **process**. Why did we use threads in this assignment instead of creating separate processes?

**Your Answer: 

A thread is a smaller execution unit inside a process, whereas a process is an active program with its own memory and resources. Threads share memory and are lighter than processes, which are heavier and demand more system resources. Because to the increased overhead, creating processes takes longer than creating threads. Because threads are more effective and appropriate for imitating CPU scheduling, we used them in this project. Multiple jobs can operate simultaneously within the same software thanks to threads.

[Write your answer here. Consider: What is a process? What is a thread? How do they differ in terms of memory, resources, creation overhead? Why are threads more suitable for this simulation?]

---

## Question 2: Ready Queue Behavior

**Question**: In Round-Robin scheduling, what happens when a process doesn't finish within its time quantum? Explain using an example from your program output.

**Your Answer: 
Round-Robin scheduling removes a process from the CPU and puts it back at the end of the ready queue if it doesn't complete within the allotted time quantum. This guarantees that every process has an equal opportunity to 


[Write your answer here. Describe the specific behavior - where does the process go? When does it run again? Give an example from your actual program output showing a process that was re-queued.]

Example from my output:
```
▶ P2 executing quantum [4000ms]
Remaining time: 3780ms
↻ P2 yields CPU for context switch

➕ P2 added to ready queue
```

**Explanation of example:**
In this instance, process P2 was assigned a 4000 ms time quantum. Nevertheless, it has 3780 milliseconds left to finish its operation. Consequently, P2 was moved to the end of the ready queue by the scheduler through a context switch.

---

## Question 3: Thread States

**Question**: A thread can be in different states: **New**, **Runnable**, **Running**, **Waiting**, **Terminated**. Walk through these states for one process (P1) from your simulation.

**Your Answer:  


[Write your answer here. For each state, explain when P1 enters that state during the simulation. Use your understanding of the code to trace through the lifecycle.]

1. **New**: P1 is in the New state when it is first created and added to the ready queue:➕ P1 added to ready queue

2. **Runnable**: After being added to the queue, P1 becomes Runnable, meaning it is ready to run but waiting for CPU time: Ready Queue: [P2 → P3 → ...]

3. **Running**: P1 enters the Running state when the scheduler assigns it CPU time: ▶ P1 executing quantum [3033ms]

4. **Waiting**: In this simulation, there is no explicit I/O waiting state. However, when P1 is not running and is waiting in the ready queue for its turn, it can be considered in a waiting-like state [P2 → P3 → ... → P1]

5. **Terminated* : P1 enters the Terminated state after completing its execution:✓ P1 finished execution! At this point, the process has fully completed and will not be scheduled again.

---

## Question 4: Real-World Applications

**Question**: Give **TWO** real-world examples where Round-Robin scheduling with threads would be useful. Explain why this scheduling algorithm works well for those scenarios.

**Your Answer:**

### Example 1:  Web servers

**Description**: 
Web servers manage several user requests at once.



**Why Round-Robin works well here**: 
Round-Robin ensures that CPU time is distributed fairly to each request, which is why it functions.


### Example 2:  Operating Systems (Time-sharing systems)

**Description**: 
Programs are run simultaneously by many users.


**Why Round-Robin works well here**: 
It increases responsiveness and gives each process the same amount of CPU time.
---

## Summary

**Key concepts I understood through these questions:**
1. The distinction between processes and threads
2. The behavior of round-robin scheduling
3. The lifespan of a thread


**Concepts I need to study more:**
1. Deadlocks
2. Advanced synchronization
