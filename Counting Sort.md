#computing #software #prog 

- a type of [[Sorting Algorithm]]
- assumes n input elements all integers in range 0 to k
- Basic Idea
	- determine for each input element x, number of elements less than x
	- information can be used to place element x directly into position in output [[array]]
	- eg. if there are 17 elements less than x, it belongs in output position 18
[[big O notation]] complexity -> O(n+k)

ex code 
```
for i <- 0 to k
	do C[i] <- 0
for j <- 0 to length[A]
	do C[A[j]] <- C[A[j]] + 1
' # n now contains the number of elements equal to i.'
for i <- 1 to k
	do C[i] <- C[i] + C[i-1]
'C[i] now contains the number of elements less than or equal to i.'
for j<- 1 to length[A] downto 1
	do B[C[A[j]]] <- A[j]
	C[A[j]] <- C[A[j]] - 1
```

list c contains the amount of numbers in list

so at register 0, shows number of 0s in the list

eg 
233354
output
01311
there are 0 1s, 1 2s, 3 3s, 1 4s, 1 5s