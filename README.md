# Parallel-Matrix-Matrix-Multiplication-with-MPI-using-Cannon-s-Algorithm

## How to install MPI on Ubuntu / Linux

1. sudo apt install openmpi-bin openmpi-dev openmpi-common openmpi-doc libopenmpi-dev

2. If above is giving an error: sudo apt install openmpi-bin libopenmpi-dev

2. mpicc --showme:version

Minimum Hardware Requirements:
1. RAM = 4GB
2. HDD = 10GB

Operating System used: Ubuntu

Language: C++


## Cannon's Matrix MAtrix Multiplication
Cannon's Matrix-Matrix Multiplication is a parallel method that divides the work across several processors or cores to quickly multiply two large matrices. The approach is especially well suited for distributed memory systems, such as networked computers. It involves dividing up the matrices into blocks and distributing them in a grid-like pattern among processors. The final result is then computed via a coordinated series of local matrix multiplications and cyclic shifts. When compared to other parallel matrix multiplication techniques, Cannon's algorithm has a lower communication overhead, making it a useful tool for high-performance computing applications.

## MPI (Message Passing Interface)
The message-passing interface (MPI) is a standardized means of exchanging messages between multiple computers running a parallel program across distributed memory.

## Cannon's Matrix MAtrix Multiplication using MPI
1. Create a text file named A.txt,
   Write the NxN Matrix of your choice
2. Create a text file named B.text,
   Write the NxN Matrix of your choice
3. Create the .c file and write code provided in cannon.c

## How to compile and run the cannon.c file
1. mpicc -o filename filename.c
2. mpirun -np 4 ./filename


## References:
1. https://iq.opengenus.org/cannon-algorithm-distributed-matrix-multiplication/#:~:text=Cannon's%20algorithm%20is%20a%20distributed,been%20shown%20to%20be%20difficult.
2. https://www.comrevo.com/2020/11/cannons-algorithm-for-matrix-multiplication.html
3. https://www.techtarget.com/searchenterprisedesktop/definition/message-passing-interface-MPI
4. OpenAI GPT-3.5 (https://www.openai.com)
