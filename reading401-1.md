[Problem Solving](https://simpleprogrammer.com/solving-problems-breaking-it-down/)

1. Read the problem completely twice.
2. Solve the problem manually with 3 sets of sample data.
3. Optimize the manual steps.
4. Write the manual steps as comments or pseudo-code.
5. Replace the comments or pseudo-code with real code.
6. Optimize the real code.

[How to Think Like a Programmer](https://www.freecodecamp.org/news/how-to-think-like-a-programmer-lessons-in-problem-solving-d1d8bf1de7d2/)

1. Understand, write down your problem or talk until you determine you fully understand the problem in front of you.
2. Plan, Analyze the problem before hacking away at the prlbme.
3. Divide, breakdown one big problem into sub-problems. Solving each sub problem one by one.
4.Connect all the sub-solutions to the original problem.
5. If stuck, debug,reasses,research the problem or bug to understand how to reasses and solve the problem.

[5 Ways of Problem Solving](https://www.mindtools.com/pages/article/newTMC_5W.htm)

1. Assemble a team
2. Define the problem
3. Ask “why” the problem is occuring
4. Ask “why” 4 more times for each answer generated
5. Know when to stop
6. Address the Root Cause
7. Monitor measures

[Event Loop](https://www.youtube.com/watch?v=8aGhZQkoFbQ)

# Call Stack

- Single threaded, only executes one piece at a time.
- Top of stock is executed bottom of stack of thrown out
- As code is executed the stack is emptied.
- Blowing the stack, overflowing the stack and exceeding it's capacity.
- Blocking, code blocks that are slow that prevent the rest of the stack from being executed.

# Concurrency & the Event Loop

- callback qeueue holds code that has finished it's execution and is pushed to the task queue to rejoin the stack.
- Event loop looks at the stack and the task queue pushes task waiting in the queue to the stack to run.

# Do not block the call stack

- blocking the call stack causes the website to not render
- rendeering happens every 16ms but only if the stack is empty
- rendering has prio over cb queue.

[The Super Mario Effect](https://www.youtube.com/watch?v=9vJRopau0g0)

- Penalty causes users to try less. If there is no penalty they will try more often ntil they have success.
- Celebrate the success and focus on the end goal.
- Holding on to the failures lower the success rate.

