1. `log2(n&-n)+1` returns the position of the rightmost set bit from right.

2. `int(log2(n)+1)` returns the number of bits in the binary representation of the given number. 

3. `x<<y` is same as `x*(2^y)`, also known as left shift operator.

4. `x>>y` is same as `x//(2^y)`, also known as right shift operator.

5. For more on operators, check this link: https://www.programiz.com/python-programming/operators

6. Binary representation of a negative is calculated by: 
	1. Finding 1's complement of number by simply inverting the bits.
	2. Adding 1 to the above number and discarding any leftover.
	Example:
	Binary representation of 6 = `110`
	Thus, 1's complement of 6 =  `001`
	Adding `1` to above, ans is= `010`

7. XOR of two bits `a^b` is `0` if bits are same and `1` if bits are different.

8. Must read page on inner functions (which are also used as decorators) : https://realpython.com/inner-functions-what-are-they-good-for/

9. For fast input try the following:
	a. 
    ```
	import sys
	n = int(sys.stdin.readline())
	arr = sys.stdin.readline().split()
	```
	b. 
    ```
	import os,io
	input = io.BytesIO(os.read(0,os.fstat(0).st_size)).readline
	n = int(sys.stdin.readline())
	arr = sys.stdin.readline().split()
	```
