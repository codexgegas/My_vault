# Time Complexity
- time Complexity is the mathematical function/relation of how long will it take as the input size increases.
- Time Complexity != time taken for the program to run.
***Example***
	which has higher number of chances of crashing the website
		 - A website with less clients like 10 or,
		 - A website with high clients like 2 million+.

==*always to look for worst case when designing the Algorithm*==

 - Always look for complexity of large data

 - we ignore the constants
 - always ignore the less dominant terms
***Example***
		 O(N^3+lo(n))
		 and size is supposed to 1 mill
		 then 
 > O((1 mill)^3+log(1 mill))
 > O((1 mill)^3+6)
>  O((1mill)^3)
	*log(6) is less compared to 1mill^3 hence ignored*


- Always Ignore the constants
	 -  ***Example***
		O(3N^3+2N^2+5N+7)
		
		> O(N^3+N^2+N)
		> O(N^3)
> Ignore the less Dominant term

	then the Time Complexity is O(N^3).


- Flow of time Complexity

	>    O(1)<O(log(N))<O(n)<O(2^n)
