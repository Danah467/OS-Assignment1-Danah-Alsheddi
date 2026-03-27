# Reflection Questions

## Instructions
Answer the following questions about your learning experience. Each answer should be **at least 5-7 sentences** and show your understanding.

---

## Question 1: What did you learn about multithreading?

**Your Answer:During this assignment I learnt that multithreading is the ability of a program to manage multiple tasks simultaneously making applications faster and more responsive. And I knew that each thread exists in its own lifecycle with the corresponding states of New, Runnable, Running, Blocked and Terminated. It was neat to observe how threads have access to common memory space—making communication between them dead simple, but also requiring care with synchronization. I also learned how the CPU switches between threads with such rapidity that it feels like everything is happening at once. Before this assignment, multithreading felt more abstract but applying it in a scheduler simulation solidified the idea. This helped me get a better perspective on concurrent execution managed by operating systems.**

[Write your answer here. Discuss specific concepts like thread creation, thread states, how threads execute concurrently, what surprised you, etc.]

---

## Question 2: What was the most challenging part of this assignment?

**Your Answer:The trickiest part for me was figuring out how to handle threads in the CPU scheduling simulation. With context switching going in every direction, it was hard to know when each process would begin, when it would end, and where it might stop. Another difficult part was to relate the logic of processes, threads, queues and maps together while ensuring all is synchronized between each other. It was also challenging to implement the waiting time feature because it needed precise records of when each process arrived in and exited from the ready queue. Then, in Java, I ran into insidious errors like redefining a duplicate variable and trying to use an undefined variable. These problems caused me to understand how complicated actual scheduling systems can be**

[Describe the specific challenge. Was it understanding the code? Implementing a feature? Using Git? Explain what made it difficult and how it relates to the course concepts.]

---

## Question 3: How did you overcome the challenges you faced?

**Your Answer:I overcome the difficulties by dividing the task into manageable chunks rather than attempting to grasp it all at once. I followed the program's flow and saw what was happening during execution by using print statements and debugging. When I ran into problems, I looked up solutions online and studied Java documentation to figure out why they happened. In order to make the connection between the theoretical ideas and the code I was producing, I also went over my class notes again. I was able to find errors and verify when the logic was sound by frequently testing the application. These techniques eventually made the task much simpler to complete.**

[Describe your problem-solving approach. Did you read documentation? Ask for help? Debug systematically? What resources did you use? What strategies worked?]

---

## Question 4: How can you apply multithreading concepts in real-world applications?

**Your Answer:Numerous real-world programs that we use on a daily basis employ multithreading. Web browsers, for instance, employ several threads to simultaneously load content, play videos, and maintain a responsive interface. To manage graphics, physics, music, and user input all at once, games require threads. In order to keep the user interface from freezing as data loads in the background, mobile applications also employ threads. I now have a better understanding of why multithreading is crucial for user experience and performance thanks to this project. Any system that wants to effectively manage several tasks can use the ideas I learnt.**

[Give specific examples from real applications you use (web browsers, games, mobile apps, etc.). Explain why threads are useful in those scenarios. Connect to what you learned in this assignment.]

---

## Additional Reflections (Optional)

### What would you like to learn more about?
**Your Answer:I want to learn more about synchronization strategies and how to avoid problems like deadlocks and race conditions. Additionally, I'm curious about thread pools and how big programs effectively handle hundreds or thousands of threads.**
[Any topics related to threading, concurrency, or operating systems that you're curious about?]

---

### How confident do you feel about multithreading concepts now?
**Your Answer:I consider myself to be Intermediate. I can use multithreading in basic applications and have a solid understanding of the fundamental ideas, but I still need additional practice with more complex subjects like concurrency control and synchronization.** 
[Rate yourself and explain: Beginner / Intermediate / Confident]

[Explain your rating - what do you understand well? What needs more practice?]

---

### Feedback on the assignment
**Your Answer:Although difficult, the homework was quite beneficial. It made me put theoretical ideas into practice, which strengthened my comprehension. The project, in my opinion, is well-designed and provides a realistic understanding of how operating systems handle scheduling.**
[Any comments about the assignment? Was it helpful? Too easy/hard? Suggestions for improvement?]
