1. **(20 points)** Order the following list of functions by the big-O notation.

![[Pasted image 20230925144522.png]]

From least amount of time to most

$1/n$, $log(log(n))$, $x^{.01}$, $\sqrt{log(n)}$, $log(5n)$, $2^{log(n)}$, $log^2(n)$, $\sqrt{n}$, $3x^{.5}$, $log(5^n)$, $log_4(n^n)$, $2nlog^2(n)$, $6nlog(n)$, $4n^\frac32$, $2^n$, $2^n+n^2+3n$, $3^n+log(2023)$, $4^n$, $(n+1)!$, $2^{2^x}$.

2. **(20 points)** Find the Asymptotic time complexity for each routine listed in this [[[Python]] code](https://gist.github.com/chenzibin2019/c5865998b87bbababee2404ca3bca3a9)
	1. O(m)
	2. O(n+m)
	3. O(2n)
	4. O(logn)
	5. O(log(nlog(m)))
	6. O(a/b)
3.  **(20 points)** This problem will demonstrate how you can use data structures and [[algorithms]] for data science.  
    In this specific case, we look into the analysis of data that has been collected by weather stations.  
    We have prepared a code skeleton ([WeatherData.pyLinks to an external site.](https://gist.github.com/chenzibin2019/316ebef1947ab2172b8dbd87006bfa28)) which will fetch temperature data from the Amherst weather station.  
    1. It is your task to finalize that code such that the function highest_temp() determines the highest temperature for a  
        certain period and the function lowest_temp() determines the lowest temperature for the same period.
    2. In addition, finalize the functions average_high() and average_low(), which have the goal to calculate  
        the average of all maximum and minimum temperatures, respectively.
4. 1. **(20 points)** A shelf contains some products sorted according to their width, e.g. |||10, 20|||.  
    
    We place more already sorted products with lesser width than the ones that are already present.
    
    e.g.     |||10, 20||1, 2, 4, 7|||.  
    Find the position of a given product (no sorting allowed and find it in O(log n) time).  
    
    e.g.     |||10, 20||1, 2, 4, 7|||
			position of product width 10 is 0
			position of product width 7 is 5
	to find the product of a certain width, we first look at the first product width in the shelf, if its larger than the width we are looking for, move onto the next shelf, repeat until you find one less than the width, next check the last width, repeating until you find a shelf with the end larger and front smaller and then implement [[binary search]] to find wanted width within the shelf.
```
inbetween = False

while inbetween == False:
	if first item > wanted > last item:
		move to next shelf
	if in between those 2 values
		inbetween = True
if wanted > middle
	move middle to middle of higher side and repeat
if wanted < middle
	move middle to middle of lower side and repeat

run until you get the position

```

5. **(20 points)** [[Merge sort]] involves recursively splitting the [[array]] into 2 parts, sorting, and finally merging them.  
    A variant of [[merge sort]] is called **3-way [[merge sort]]** where instead of splitting the [[array]] into 2 parts we split it into 3 parts. As shown in the MergeSort code, it recursively breaks down the arrays to subarrays of size half. Similarly, the 3-way [[Merge sort]] breaks down the arrays into subarrays of size one-third.  
      
    In this question, you need to implement the 3-way [[Merge sort]] algorithm in function [[[merge Sort]]](https://gist.github.com/chenzibin2019/15c6ec906a43506bcce9e15b2131f634)in descending order. During the sorting, count the number of comparisons in each merge stage.