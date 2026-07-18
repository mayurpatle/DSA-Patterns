### PATTERN 2 – Subarray Sum / HashMap + Prefix

#### Sum = K (count)

Store the count  in the  hashmap 
initialize the map with  {0, 1} - means the  sum of  the  subaaray starting  from 0th index is freq 1 as obvious    

#### Problems : 

- LC560. Subarray Sum Equals K

count all the  subarray with sum  =  k , loop over the  array and  take the sum and  store the sum  in the map as counts 
if sum - k is there add its freq to the  the  ans. 

#### Sum = K (longest subarray)


#### Problems : 

- LC325. Maximum Size Subarray Sum Equals K


