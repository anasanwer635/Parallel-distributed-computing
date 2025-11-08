1. broadcast.py

Demonstrates MPI broadcast communication using mpi4py.

The root process (rank 0) initializes a variable and broadcasts it to all other processes.

Every process prints the received shared value.

Illustrates one-to-many data sharing in MPI.


broadcast

2. pointToPointCommunication.py

Shows point-to-point message passing between multiple processes using send() and recv().

Process 0 sends data to process 4.

Process 1 sends data to process 8.

Destination processes receive and display the transmitted values.

Demonstrates direct communication between specific pairs of processes.


pointToPointCommunication

3. gather.py

Implements MPI gather operation to collect results from all processes to the root.

Each process computes (rank + 1)² and sends it to the root (rank 0).

The root gathers all results and prints data received from each process.

Illustrates many-to-one communication.


gather

4. scatter.py

Demonstrates MPI scatter operation to distribute an array among processes.

The root (rank 0) has an array of integers.

Each process receives a single element from the array.

Useful for splitting large data sets across multiple workers.


scatter

5. deadLockProblems.py

Shows an example of deadlock in MPI using bidirectional send()/recv() between two processes.

Process 1 and process 5 both try to send messages simultaneously before receiving.

If not carefully ordered, this leads to a deadlock situation.

Demonstrates the importance of proper message ordering and synchronization.


deadLockProblems
