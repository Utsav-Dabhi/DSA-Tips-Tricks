# DSA-Tips&Tricks

If you have been practising DSA, you might have encountered the problem of what the worst-case time complexity of your solution could be.

There is an easy way to find out by simply looking at the constraints of your problem. You're probably wondering how this is possible.

<br/>
Let's understand this:<br/>
A typical computer takes 1 second for 10^8 computations.<br/>
i.e 1 sec = 10^8 computations<br/><br/>

So the expected worst-case complexity for your problem should be -
| No of Operations | Complexity | Approx |
|--|--|--|
|10<sup>12</sup>|O( $\sqrt{N}$ )||
|$10^8$|O( N )||
|$10^6$|O( N * $log{N}$ )|2 * $10^7$|
|$10^5$|O(N * $\sqrt{N}$)|3 * $10^7$|
|$10^4$|O( $N^2$ )|$10^8$|
|$10^3$|O( $N^2$ * $\sqrt{N}$ )|3 * $10^6$|
|N $\leq$ 25|O( $2^N$ )|
|N $\leq$ 10|O( N! )|

<br/><br/>
And you may use one of the following data structures accordingly.
<br/>

|Data Structure|TC|
|--|--|
|Hashmap|O( N * $log{N}$ )&nbsp;&nbsp;&nbsp;{Ordered}<br/>O( N )&nbsp;&nbsp;&nbsp;&nbsp;{Unordered}|
|Heap|O( N * $log{N}$ )|
|Binary Search|O( $log{N}$ )|
|Sorting algos|O( N * $log{N}$ )|
|Backtracking|O( $2^N$ )|
|Permutations|O( N! )|
