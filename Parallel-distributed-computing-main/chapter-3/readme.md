1. communicating_with_pipe.py

Demonstrates inter-process communication (IPC) using multiprocessing.Pipe.

One process sends numbers 0–9 through a pipe.

Another process receives them, squares each number, and sends results to a second pipe.

The main process prints squared values until the stream ends.

Shows data flow and transformation through connected pipes.


communicating_with_pipe

2. communicating_with_queue.py

Implements the Producer–Consumer model using multiprocessing.Queue.

The producer generates random integers and places them into the queue.

The consumer retrieves and prints each item until the queue becomes empty.

Demonstrates safe sharing of data among processes using queues.


communicating_with_queue

3. killing_processes.py

Shows how to terminate and monitor processes.

A process runs a loop printing numbers, and the parent process terminates it mid-execution.

Displays the process status before, during, and after termination.

Useful for understanding process lifecycle control (start(), terminate(), join(), and exitcode).


killing_processes

4. naming_processes.py

Illustrates assigning custom names to processes.

One process is created with a user-defined name and another with a default name.

Each process prints its start and exit messages.

Demonstrates custom identification of processes in large multiprocessing systems.


naming_processes

5. process_in_subclass.py

Demonstrates creating a custom process class by subclassing multiprocessing.Process.

Each subclass instance overrides the run() method.

Ten processes are created and executed sequentially.

Useful for object-oriented process design.


process_in_subclass

6. process_pool.py

Implements a process pool for parallel computation.

Defines a simple function that returns the square of each number.

A pool of 4 worker processes maps the function over inputs 0–99.

Demonstrates data parallelism and process pooling using multiprocessing.Pool.


process_pool

7. processes_barrier.py

Shows process synchronization using a Barrier and Lock.

Two processes wait at a barrier before proceeding together.

Others run without synchronization for comparison.

Demonstrates coordinated execution and time alignment between processes.


processes_barrier

8. run_background_processes.py

Explains the difference between daemon and non-daemon processes.

One process runs as a background daemon; another runs normally.

Daemon process stops when the main process exits.

Illustrates lifetime dependency of background processes.


derom

9. spawning_processes.py

Shows spawning multiple processes in a loop.

Each process executes a function that prints its index and output.

Demonstrates independent process creation and controlled joining.

Useful for understanding process instantiation and sequential joins.


spawning_processes

10. derom.py

Another version of daemon vs non-daemon demonstration.

Similar to run_background_processes.py but with slightly different iteration behavior.

Confirms how daemon processes end automatically when the main program exits.


run_background_processes
