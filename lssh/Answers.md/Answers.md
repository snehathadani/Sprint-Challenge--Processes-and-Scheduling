List all of the main states a process may be in at any point in time on a standard Unix system. Briefly explain what each of these states mean.
Start : process is initialized
Ready: Awiats the operating system to allocate to the processers. Some proceeses may already be running and join this state if as directed by scheduler, which replaces them with other process
Running: Process is in this state when it is prepared to execute OS scheduler's instructions
Waiting: Awaits the necessary requirement for continuity.
Exit: Exits and is removed from main memory



What is a Zombie Process? How does it get created? How does it get destroyed?
The process is executed and still remains in OS until its reported to its' parent process. Thus it can not be removed and can not be further scheduled, until exit status has been confirmed.
parent process can remove the zombie process by calling wait()! Once the parent gets notified, child process gets removed.



Describe the job of the Scheduler in the OS in general.
scheduler aloocates system resources to many different tasks. It determines queue priority and allocates appropriate time for each task.


Describe the benefits of the MLFQ over a plain Round-Robin scheduler.
Round Robin scheduling first in first out and is a queue. So one can't prioratize tasks.
MLFQ can lower the priority, or manually increase the priority. SO the system is fair and long running processes get penalized by moving to lower priority, because single process cant take over the system.
