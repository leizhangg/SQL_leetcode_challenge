<img src = "https://github.com/leizhangg/SQL_leetcode_challenge/blob/main/img/585_1.png">
<img src = "https://github.com/leizhangg/SQL_leetcode_challenge/blob/main/img/585_2.png">

### Solution 1:  
The problem here is to find the sum based on 2 creteria.  
#1 is the have the same tiv_2015 value at least once, which means the tiv_2015 has to occure at least twice.   
#2 is the pair of Lat and Lon has to be unique, which means the the combination of Lat and Lon has to occure only once.  

In this case, we could use COUNT()OVER() window function to count the occurance of tiv_2015 and Lat, Lon,  
then select the tiv_2015 > 1 and Lat, Lon =1

<img src = "https://github.com/leizhangg/SQL_leetcode_challenge/blob/main/img/585_solution_1.png">

### Solution 2:
Simply use HAVING(), COUNT() with 2 subqueies. One thing need to be careful is the combination of Lat and Lon.    
Here I use CONCAT to combine them together

<img src = "https://github.com/leizhangg/SQL_leetcode_challenge/blob/main/img/585_solution_2.png">

It shows that Solution 2 is faster with 811ms runtime.

<img src = "https://github.com/leizhangg/SQL_leetcode_challenge/blob/main/img/585_result.png">
