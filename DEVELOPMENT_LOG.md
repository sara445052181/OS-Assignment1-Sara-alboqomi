# Development Log

## Instructions
Document your development process as you work on the assignment. Add entries showing:
- What you worked on
- Problems you encountered
- How you solved them
- Time spent

**Requirements**: Minimum 5 entries showing progression over time.

---

## Example Entry Format:

### Entry 1 -[March 29, 2026, 3:00 PM]
**What I did**: Set up the project and ran the initial code

**Details**: 
- Opened the project in VS Code
- Updated my student ID in the code
- Ran the program successfully
- Observed how processes are created and executed

  
**Challenges**: Understanding how threads are connected to processes

**Solution**: Watched a short tutorial and understood the difference. 

**Time spent**: 3.5 hours

---

## Your Development Log:

### Entry 2 - [March 29, 2026, 7:00 PM]

**What I did**: Implemented Feature 1 (Process Queue visualization)

**Details**:
Examined the behavior of the ready queue
Print statements were added to show the queue.
Confirmed output complies with FIFO scheduling

**Challenges**: Formatting the output of the queue

**Solution**:  Used loops and string formatting

**Time spent**: 1.5 hours

---

### Entry 3 - [March 30, 2026, 3:00 PM]
**What I did**: Implemented Feature 2 (Context Switch Counter)

**Details**: 
-Added contextSwitches variable
- Incremented it before each thread execution
- Printed final result

**Challenges**: Finding correct placement of counter

**Solution**:  Placed it before start() after understanding scheduling 

**Time spent**: 1 hour

---

### Entry 4 -  [March 30, 2026, 4:00 PM]
**What I did**: Implemented Feature 3 (Waiting Time calculation)

**Details**: 
- Added arrivalTime and waitingTime variables
- Calculated waiting time before execution
- Updated arrival time after each run

**Challenges**: Errors with process variable not defined

**Solution**: Fixed by defining process using processMap


**Time spent**: 2 hours

---

### Entry 5 - [March 30, 2026, 7:00 PM]
**What I did**: Tested program and wrote answers

**Details**: 
- Verified output correctness
- Observed process re-queue behavior
- Completed assignment answers


**Challenges**: Understanding thread states

**Solution**: I relied on actual execution rather than theory, which made the concept clearer.


**Time spent**:  1.5 hours

---

---


## Summary

**Total time spent on assignment**: [10 hours]

**Most challenging part**: 

Understanding how Round-Robin scheduling uses threads—particularly tracking process movement in the ready queue and accurately computing waiting time—was the most difficult aspect. It was also challenging to debug problems like undefined variables and improper code placement (like arrivalTime updates).

**Most interesting learning**: 
Seeing how processes are scheduled in real time and how time quantum is used to provide each task a fair share of CPU was the most fascinating aspect. The concept became much evident when one saw the output's ready queue modifications and context switching.


**What I would do differently next time**: 


The next time, in order to prevent mistakes, I would thoroughly outline the implementation before coding and test each feature independently. Additionally, I would trace variables step-by-step earlier in the process to enhance my debugging methodology.
