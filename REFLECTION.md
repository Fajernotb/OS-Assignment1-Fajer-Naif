# Reflection Questions

## Instructions
Answer the following questions about your learning experience. Each answer should be **at least 5-7 sentences** and show your understanding.

---


## Question 1: What did you learn about multithreading?

I discovered that multithreading enables the simultaneous execution of several tasks within a single process. Because every thread has access to the same memory, communication is quicker than with processes. Additionally, I was aware of a thread's creation, execution, waiting, and termination phases. One key idea was how the CPU uses algorithms like Round Robin to schedule threads. The speed at which the CPU switches between threads and how context switching operates shocked me. I was able to see how operating systems effectively handle certain jobs thanks to this project. In general, I developed a useful comprehension of thread behavior.

[Write your answer here. Discuss specific concepts like thread creation, thread states, how threads execute concurrently, what surprised you, etc.]

---

## Question 2: What was the most challenging part of this assignment?

The waiting time element was the hardest to develop. The challenge was figuring out how to compute waiting time accurately without using private variables directly. At first, I attempted to change variables directly, which led to mistakes. Understanding how threads interact with the scheduler loop presented another difficulty. It was also challenging to debug the issues caused by duplicate variables and improper code placement. This problem relates to operating system concepts of thread synchronization and encapsulation.

## Question 3: How did you overcome the challenges you faced?

--I overcame these difficulties by segmenting the issue into manageable chunks. I started by going over the lecture notes and textbook ideas around scheduling and threads. I then thoroughly examined the code to comprehend how each component functions. Additionally, I employed debugging strategies like printing interim values. When I ran into problems, I carefully analyzed the error messages to figure out what was wrong. I addressed each issue one at a time using a methodical technique. Using this approach, I was able to effectively finish the task over time.-

## Question 4: How can you apply multithreading concepts in real-world applications?

Numerous real-world applications make extensive use of multithreading. Web browsers, for instance, use several threads to run programs, play videos, and load webpages all at once. Mobile apps are another example, where background operations like data downloads are carried out on different threads. Threads are used in games to manage physics, rendering, and user input simultaneously. This guarantees quickness and seamless operation. I saw how threads mimic CPU scheduling in this assignment, which is comparable to how actual operating systems handle jobs.

[Give specific examples from real applications you use (web browsers, games, mobile apps, etc.). Explain why threads are useful in those scenarios. Connect to what you learned in this assignment.]

---

## Additional Reflections (Optional)

### What would you like to learn more about?

I want to know more about preventing race situations and thread synchronization.

---

### How confident do you feel about multithreading concepts now?

[Rate yourself and explain: Beginner / Intermediate / Confident]

[Explain your rating - what do you understand well? What needs more practice?]

---

### Feedback on the assignment

[Any comments about the assignment? Was it helpful? Too easy/hard? Suggestions for improvement?]
