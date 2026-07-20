### PATTERN 2 – Subarray Sum / HashMap + Prefix

#### Sum = K (count)

Store the count  in the  hashmap 
initialize the map with  {0, 1} - means the  sum of  the  subaaray starting  from 0th index is freq 1 as obvious    

#### Problems :

- LC560. Subarray Sum Equals K

count all the  subarray with sum  =  k , loop over the  array and  take the sum and  store the sum  in the map as counts 
if sum - k is there add its freq to the  the  ans. 

*Similar problems : LC974 , LC1248 , LC930*

#### ✅ Sum = K (longest subarray)

here we have to track the  indexes of the sum so that we can calculate the  length

#### Problems :

- LC325. Maximum Size Subarray Sum Equals K

it is the same as the subarray sum equals k but  here  we  store the index  in place of coutn of the  running sum and  if  sum - k exists  is the  map we store curr index - index at sum - k and  store it  in the global max. 

#### Binary Subarray :

#### ✅ Transform pattern

here we tranform the elements of the  array 

#### Problems :

- LC525. Contigous array:

here we transfrom all the 0's in the  array to -1 so that sum becomes 0 and we conform equal number of zeros and ones in the array and then by finding the first index of the sum we cal the  max  len. 

*Similar problems : LC1124 , LC2483 , LC1546*

#### ✅ Divisiblity (mod  K ) :

Two subarrays with same (prefix mod k) have sum divisible by k
How to handle negative remainders : Normalize mod: ((prefix%k)+k)%k

#### Problems :

- [ ] LC974. Subarrays sum divisible by K : 
    here we store the remaindes in the  mod array and the  ans is the  sum of  all the  remainders , remainder 0 will have  freq of  1 as always and then we calculate the remainder by  ((rem + x  %k)+k)%k where x is the element  in the array then we add the  freq of the remainder 
    Similar Problems : 
  - [ ] LC523. Continous Subarray Sum
  - [x] LC1590. Make Sum divisible by P : *here  we need to find the subarray whoose sum have the same  remainder asthe  whole  sum of  the  array has  when divided by p.*
  - [ ] LC2364. Count number of bad Pairs