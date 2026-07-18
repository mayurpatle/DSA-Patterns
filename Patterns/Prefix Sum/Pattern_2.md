### PATTERN 2 – Subarray Sum / HashMap + Prefix

#### Sum = K (count)

Store the count  in the  hashmap 
initialize the map with  {0, 1} - means the  sum of  the  subaaray starting  from 0th index is freq 1 as obvious    

#### Problems : 

- LC560. Subarray Sum Equals K

count all the  subarray with sum  =  k , loop over the  array and  take the sum and  store the sum  in the map as counts 
if sum - k is there add its freq to the  the  ans. 

*Similar problems : LC974 , LC1248 , LC930*


#### Sum = K (longest subarray)

here we have to track the  indexes of the sum so that we can calculate the  length


#### Problems : 

- LC325. Maximum Size Subarray Sum Equals K

it is the same as the subarray sum equals k but  here  we  store the index  in place of coutn of the  running sum and  if  sum - k exists  is the  map we store curr index - index at sum - k and  store it  in the global max. 


#### Binary Subarray : 

#### Transform pattern  

here we tranform the elements of the  array 

#### Problems : 

- LC525. Contigous array:

here we transfrom all the 0's in the  array to -1 so that sum becomes 0 and we conform equal number of zeros and ones in the array and then by finding the first index of the sum we cal the  max  len. 

*Similar problems : LC1124 , LC2483 , LC1546*







