# Task Prioroties
In this example we will focus on task priorities. We have one high intensity task which uses much of the CPU and one sparse intensity task which mainly uses I/O. The task here is to handle the priorities of the tasks to make sure that no tasks miss the deadline. You will also learn how to measure time in FreeRTOS to evaluate the feasibility of a real-time system in practice.

Create a new task "prioritysettask" which: 

Sets the priority of "communicationtask" to 4 in case its execution time is more than 1000 milliseconds (Hint: look at vApplicationTickHook() to measure it)

Sets the priority of "communicationtask" to 2 in case its execution time is less than 200 milliseconds (Hint: look at vApplicationTickHook() to measure it)

-Provide a screenshot of the execution and answer the following questions in a report:

Why is "matrixtask" using most of the CPU utilization?

Why must the priority of "communicationtask" increase in order for it to work properly

What happens to the completion time of "matrixtask" when the priority of "communicationtask" is increased?

How many seconds is the period of "matrixtask"? (Hint: look at vApplicationTickHook() to measure it)  


