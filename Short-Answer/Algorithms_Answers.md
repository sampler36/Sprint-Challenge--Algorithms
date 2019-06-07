Add your answers to the Algorithms exercises here.
```
a) a = 0  #O(1)
    while (a < n * n * n) #O(n)
     a = (a + n )* n #O(n)
There is one while loop which has a time complexity of O(n). I  multiplied the nested time complexities to get O(1) * O(n) = O(n). O(n) dominates the O(1) (from a = O);
O(n) would be the time complexity of the entire code.
if n = 2 then it would take 2 iterations for the loop to break
if n = 10 then thats  10 iterations
meaning the performance will grow linearly and in direct proportion to the size of the input data set


b) sum = 0   #O(1)
    for (i = 0; i < n; i++)    #O(n)   
      for (j = i + 1; j < n; j++)    #O(n)
        for (k = j + 1; k < n; k++)      #O(n)
          for (l = k + 1; l < 10 + k; l++)  #O(n)
            sum++   

For all of the nested for loops you multiply their time complexities to get O(n) * O(n) * O(n) * O(n) * O(1) = O(n^4). This dominates O(1) from the first line, O(n^4) becomes the overall time complexity.
