						Design & Analysis of Algorithms
												CS324


----------------------------------------------------


 #  #Introduction 

 ## Why do we study Algorithms?
 
-  Algorithm is a step-wise representation of a solution to a given problem.
-  In Algorithm the problem is broken down into smaller pieces or steps hence, it is easier for the programmer to convert it into an actual program.
- Its important for other branches of computer science.
 - it plays a key role in modern technology
 - its challenging and fun.
 - It is easy to understand.
---

### Disadvantages of Algorithms:

-   Writing an algorithm takes a long time so it is time-consuming.
-   Branching and Looping statements are difficult to show in Algorithms.

---

 # ==***Perhaps the most most important principle for the good algorithm designer is to refuse to content***==
		 - Alfred V. Aho
	 
*****In simple terms its about can we do it better!!!*

Example of Algo

A Python Program to add 3 numbers

# Python3 program to add three numbers
# with the help of above designed
# algorithm


if __name__ == "__main__":

	
	num1 = num2 = num3 = 0

	# Variable to store the resultant sum
	sum = 0

	# Take the 3 numbers as input
	num1 = int(input("Enter the 1st number: "))

	num2 = int(input("Enter the 2nd number: "))

	num3 = int(input("Enter the 3rd number: "))

	# Calculate the sum using + operator
	# and store it in variable sum
	sum = num1 + num2 + num3

	# Print the sum
	print("\nSum of the 3 numbers is:", sum)




		![[Pasted image 20220121111757.png]]

# Difference between Algorithm, Pseudocode and Program
**Algorithm:**
An Algorithm is used to provide a solution to a particular problem in form of well-defined steps. Whenever you use a computer to solve a particular problem, the steps which lead to the solution should be properly communicated to the computer

---
**Pseudocode:**  
It is one of the methods which can be **used to represent an algorithm for a program**. It **does not have a specific syntax** like any of the programming languages and thus cannot be executed on a computer. There are several formats which are used to write pseudo-codes and most of them take down the structures from languages such as **C, Lisp, FORTRAN, etc.**

---
**Program:**  
A program is a set of instructions for the computer to follow. The machine can’t read a program directly, because it only understands machine code. But you can write stuff in a computer language, and then a compiler or interpreter can make it understandable to the computer.

---

# Analysis of Algorithms
 the **analysis of algorithms** is the process of finding the computational complexity of algorithms—the amount of time, storage, or other resources needed to execute them.
 An algorithm is said to be efficient when this function's values are small, or grow slowly compared to a growth in the size of the input. Different inputs of the same size may cause the algorithm to have different behavior, so [best, worst and average case](https://en.wikipedia.org/wiki/Best,_worst_and_average_case "Best, worst and average case") descriptions might all be of practical interest. When not otherwise specified, the function describing the performance of an algorithm is usually an [upper bound](https://en.wikipedia.org/wiki/Upper_bound "Upper bound"), determined from the worst case inputs to the algorithm.
 
 **_Given two algorithms for a task, how do we find out which one is better?_**  
One naive way of doing this is – implement both the algorithms and run the two programs on your computer for different inputs and see which one takes less time. There are many problems with this approach for analysis of algorithms.  
1) It might be possible that for some inputs, first algorithm performs better than the second. And for some inputs second performs better.  
2) It might also be possible that for some inputs, first algorithm perform better on one machine and the second works better on other machine for some other inputs.


   > Algo find-max(A, n)
					   >  A- Array  A={4,4,5,2,5,2,5,6,7,} n=10
 					   >  n-size
					   >  R_t= f(n)

---

## Asymptotic Analysis
[Asymptotic Analysis](http://en.wikipedia.org/wiki/Asymptotic_analysis) is the big idea that handles above issues in analyzing algorithms. In Asymptotic Analysis, we evaluate the performance of an algorithm in terms of input size (we don’t measure the actual running time). We calculate, how the time (or space) taken by an algorithm increases with the input size.

***Asymptotic Analysis is not perfect, but that’s the best way available for analyzing algorithms***

---

### Running time
 -  time taken by the algo increase with input size
	 >R_t =F(n)
- Average case is often difficult to determine
- Worst is more focused
	  
		![[Pasted image 20220121112030.png]]

---
### ==Experimental Studies==
 
**Code**
 > // Online C compiler to run C program online
#include <stdio.h>
#include <time.h>
// for clock_t, clock( ), CLOCKS_PER_SEC
#include <unistd.h>
int main( ) {
int i=0, sum=0;
double time_spent = 0.0;
clock_t begin = clock();
printf("Hello world");
for (i=0; i<100; i++)
sum=sum+i;
printf("The value of sum = %d", sum);
clock_t end = clock();
time_spent += (double)(end - begin) /CLOCKS_PER_SEC;
    printf("\nThe elapsed time is %f seconds",  time_spent);
    return 0;
}

**Output**
> Hello world The value of sum = 4950
The elapsed time is 0.000070 seconds

==Limitations OF Experiments==
 - Its necessary to implement the algo which is usually difficult

---
===Theoritical Analysis==

![[Pasted image 20220121115736.png]]
