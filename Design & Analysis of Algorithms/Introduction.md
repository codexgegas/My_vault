						Design & Analysis of Algorithms
												CS324


----------------------------------------------------


 ## #Introduction 

 ## Why do we study Algorithms?

 - Its important for other branches of computer science.
 - it plays a key role in modern technology
 - its challenging and fun.

 # ==***Perhaps the most most important principle for the good algorithm designer is to refuse to content***==
		 - Alfred V. Aho
	 
*****In simple terms its about can we do it better!!!*

		![[Pasted image 20220121111757.png]]
 
 ## Analysis the Algorithms
  - An Algo is a step-by-step Procedure for solving a problem in a finite amount of time.

   > Algo find-max(A, n)
					   >  A- Array  A={4,4,5,2,5,2,5,6,7,} n=10
 					   >  n-size
					   >  R_t= f(n)
					
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
