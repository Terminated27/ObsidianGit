#info #prog #matlab 

# software
- [[Arrays]] are a fundamental [[data structure]] that stores a collection of elements, typically of the same data type, in contiguous memory locations.
- Elements in an [[array]] are accessed by their index, starting from 0 for the first element.
- [[Arrays]] have constant-time access but may require resizing if their size exceeds capacity.

# hardware
![[Pasted image 20230908112222.png]]
# [[MATLAB]]
## how to make array in [[MATLAB]]
row array
`[ 1 2 3 4 ]`
column array
`[ 1; 2; 3; 4 ]`
[[Matrix]]

can use commas but don't need to
can make an array with functions inside
`[x+2 y*3 z/4]`
just need to define variables

## operations on array
`[1 2 3] .* [1 2 3]`

= `[1 4 9]`
need the dot, otherwise try to multiply array, incorrect compared to desired, multiplying each point in array by corresponding number
can do this with multiplication, division, any operation really

addition and subtraction are simply + or -, no dot

sum the whole array, use sum() command