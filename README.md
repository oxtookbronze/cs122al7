# cs122al7
I am going to publish all my asssignments so that no one has to suffer in the way that I am suffering

## 7.11 LAB: Utilization

In this lab, you will be writing a program that reports the utilization of a microcontroller consisting of 3 tasks with periods of 150ms, 200ms, and 450ms for task 0, task 1, and task 2, respectively. Utilization is calculated as Utilization = ( (H/T1.period)T1.WCET + (H/T2.period)T2.WCET + … + (H/Tn.period)*Tn.WCET ) / H from zyBooks chapter 7.4. Where H is the hyperperiod (LCM of tasks' period) and will be equal to 1800ms in this lab. In oreder to calculate the utilization you will need to get the WCET of each task. Use TimerRead() function to get the current system time in ms for WCET calculations.

In this lab, the main loop will only iterate for hyperperiod/tasksPeriodGCD times, at the end of the main loop calculate and print the utilization of the microcontroller.

TAs will manually grade your code to functionality and for clean readable simple consistent code style. So just use "Submit" to turn in your code; there's no auto-grading though and you'll see 0 points, but submitting enables the TAs to see your submission. They'll grade the latest submission.

## 7.12 LAB: Jitter time
In embedded systems jitter time is the difference between the time a task is ready for the execution and the time the task is actually executed. This delay is caused by the latency of the computations in other tasks. In this lab, you will write a program that reports the jitter time of the tasks in the system.

There are three tasks in the system, you need to modify the task scheduler's code so that whenever a task is scheduled for execution, it prints the jitter time of the task. Use TimerRead() function to get the current system time in ms.

TAs will manually grade your code to functionality and for clean readable simple consistent code style. So just use "Submit" to turn in your code; there's no auto-grading though and you'll see 0 points, but submitting enables the TAs to see your submission. They'll grade the latest submission.
