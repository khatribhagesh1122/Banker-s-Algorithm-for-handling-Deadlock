Ques. There are 5 processes and 3 resource types, resource A with 10 instances, B with 5 instances and C with 7 instances. Consider following and write a c code to find whether the system is in safe state or not?

Available	Processes	Allocation	Max
A	B	C		A	B	C	A	B	C
3	3	2	P0	0	1	0	7	5	3
	P1	2	0	0	3	2	2
	P2	3	0	2	9	0	2
	P3	2	1	1	2	2	2
	P4	0	0	2	4	3	3

-----

Banker's algorithm is a deadlock avoidance algorithm. It is named so because this algorithm is used in banking systems to determine whether a loan can be granted or not.
Consider there are n account holders in a bank and the sum of the money in all of their accounts is S. Every time a loan has to be granted by the bank; it subtracts the loan amount from the total money the bank has. Then it checks if that difference is greater than S. It is done because, only then, the bank would have enough money even if all the n account holders draw all their money at once.
Banker's algorithm works in a similar way in computers.
Whenever a new process is created, it must specify the maximum instances of each resource type that it needs, exactly.
