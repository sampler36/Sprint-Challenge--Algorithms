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
          for (l = k + 1; l < 10 + k; l++)  #O(1)
            sum++   

For all of the nested for loops you multiply their time complexities to get O(n) * O(n) * O(n) * O(1) * O(1) = O(n^3). This dominates O(1) from the first line, O(n^3) becomes the overall time complexity.


c)  def bunnieEars(bunnies)
      if bunnies == 0:
        return 0
      return 2 + bunnieEars(bunnies-1)

This function calls itself and it equates the input to the output so the time complexity is O(n).


Excersice II 
a) _n_story = x
   _f_ = 
   if _f_ is higher hence the number 
   of eggsdropped is  minimized
   lets say x is room/floor (f) this means f is the safe heaven
   if f < / <= currentfloor return safe drop
   else return egg broken and vise vessa
  
def eggs_drop(n, floor):
    if floor >= f:
      print("eggs drops")
      floor = f//2
    else:
      print("eggs are safe")
      return floor

Using binary search means we splitting the search in 2s everytime we try to find the safer room which is less or equal to f. So f will be our middle index [] and time complexity would be O(log(n)) 