1. IPC.py

Implements the Producer–Consumer problem using the multiprocessing module.

Two producers create items and place them in a shared Queue.

Two consumers retrieve and process items from the same queue.

Demonstrates inter-process communication (IPC) and synchronization between processes.

2. MPI.py

Shows basic multiprocessing by creating two independent processes.

Each process prints a message.

Demonstrates how to start, run, and join multiple processes.

3. ProcessCreationAndManagement.py

Creates and manages two separate processes performing different tasks.

One process calculates the square of a number.

The other calculates the cube of the same number.

Illustrates parallel execution of processes.

4. synchronization.py

Demonstrates thread synchronization using a semaphore and a thread pool.

Multiple threads attempt to access a shared resource.

A semaphore ensures that only one thread accesses the resource at a time.

Shows safe concurrent execution with ThreadPoolExecutor.
