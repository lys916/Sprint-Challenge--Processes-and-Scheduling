1. List all of the main states a process may be in at any point in time on a
   standard Unix system. Briefly explain what each of these states mean.

A process can be in a blocked state or a execution state. When a process is in a blocked state, it gets dequeued to a special queue that handles all the blocked processes. After the process is done with the blocked queue, it gets sent back to the regular queue by the scheduler and continue getting the process time.

2. What is a Zombie Process? How does it get created? How does it get destroyed?

A Zombie Process is a process that has been done executing but the exit status has not been cleaned up by the parent process yet.

3. Describe the job of the Scheduler in the OS in general.

A scheduler is responsible for managing processes. It has the ability to send and move processes around to get execution time.

4. Describe the benefits of the MLFQ over a plain Round-Robin scheduler.

It helps spread out processes into different queque for processing depending on the process time needed for each process. This way, the processes that don't need a lot of time to finish will not have to wait for the longer processes to finish. It gives a fair amount of time for each process in each queque.

