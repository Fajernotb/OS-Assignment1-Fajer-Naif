# Development Log

### Entry 1 - March 25, 2026, 3:00 PM
What I did: Set up the project and explored the code

Details:
- Forked the repository and cloned it locally
- Added my student ID to the code
- Ran the program successfully to understand output behavior

Challenges:
Understanding how threads are created and executed

Solution:
Reviewed the run() method and basic thread lifecycle

Time spent: 2 hours

---

### Entry 2 - March 26, 2026, 5:00 PM
What I did: Implemented Feature 1 (Priority)

Details:
- Added priority variable to Process class
- Modified constructor to include priority
- Generated random priority in main method
- Displayed priority in ready queue

Challenges:
Understanding how to pass new parameters in constructor

Solution:
Reviewed Java constructors and parameter passing

Time spent: 2 hours

---

### Entry 3 - March 27, 2026, 6:30 PM
What I did: Implemented Feature 2 (Context Switch Counter)

Details:
- Added global counter variable
- Incremented counter before each thread execution
- Displayed total context switches at the end

Challenges:
Finding correct location to increment counter

Solution:
Analyzed scheduling loop and placed counter before start()

Time spent: 1.5 hours

---

### Entry 4 - March 28, 2026, 4:00 PM
What I did: Implemented Feature 3 (Waiting Time)

Details:
- Added waitingTime and creationTime variables
- Created methods to update and retrieve waiting time
- Calculated waiting time before execution

Challenges:
Accessing private variables caused errors

Solution:
Used encapsulation by adding getter and update methods

Time spent: 2.5 hours

---

### Entry 5 - March 29, 2026, 7:00 PM
What I did: Final testing and debugging

Details:
- Fixed errors in waiting time calculation
- Ensured no duplicate variables
- Verified output correctness
- Tested multiple runs

Challenges:
Debugging runtime errors

Solution:
Used step-by-step debugging and print statements

Time spent: 2 hours

---

## Summary

Total time spent on assignment: 10 hours

Most challenging part:
Implementing waiting time correctly due to encapsulation issues

Most interesting learning:
Understanding how threads simulate CPU scheduling

What I would do differently next time:
Plan features before implementation

