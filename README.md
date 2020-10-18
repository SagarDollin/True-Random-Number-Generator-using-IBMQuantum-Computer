# True-Random-Number-Generator-using-IBMQuantum-Computer
Remember how a qubit in an equal superposition can collapse to either a 1 or a 0 after measuring? Well its not possible to determine what state it will collapse before actually measuring it, so we can use this property to generate truly random numbers.

So let's quickly dive into how I have designed this algorithm. But first of all some basic knowledge we need as stated below:
1) A qubit is in equal superposition after you apply a Hadamard gate on it, given that it was in state 0 or 1 initially.
2) There is no way to determine this equal superposition will collapse to 1 or a 0 before actually measuring it.
3) The above property can be used to generate random numbers, for example, if I want a random number between 0 and 1 , I need a 1 qubit then apply a hadamard gate on it and then run measure it , so the outcome you get is either 0 or 1 and there is no way to determine which outcome you will get. Now if I want a random number between 0 and 3 I take a qubit apply hadamard on it and then measure it and repeat the same once again. By doing this I get the possible outputs as 00,01,10,11 and there is no way to tell which one i will get for sure.

similary if I want a random number between 0 to (2^n)-1 i do the do the same process n times and i will get a random number between the expected range. Note that this is not a psuedo random number its a true random number.

Now, coming to the source code, Im using Qiskit packages to run the above algorithm in python language and I'm running it on a Real IBM Quantum Computer thanks to IBM and Qiskit for making this so easy.
If you are familiar with Qiskit then you should not have any trouble understanding the code , if not then Qiskit has some amazing resources from where you can learn alot about Quantum Computing.
