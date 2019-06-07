Add your answers to the Algorithms exercises here.

a) a = 0  #O(1)
while (a < n * n * n) #O(n)
a = (a + n )* n #O(n)
There is one loop which has a time complexity of O(n). You multiply the nested time complexities to get O(1) * O(n) = O(n). O(n) dominates the O(1) (from a = O);
O(n) would be the time complexity of the entire code.
if n = 2 then it would take 2 iterations for the loop to break
if n = 10 then thats  10 iterations
meaning the performance will grow linearly and in direct proportion to the size of the input data set

