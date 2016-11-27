# LRU_Cache
Least Recently Used (LRU)
Discards the least recently used items first. This algorithm requires keeping track of what was used when, which is expensive if one wants to make sure the algorithm always discards the least recently used item. General implementations of this technique require keeping "age bits" for cache-lines and track the "Least Recently Used" cache-line based on age-bits. In such an implementation, every time a cache-line is used, the age of all other cache-lines changes. LRU is actually a family of caching algorithms with members including 2Q by Theodore Johnson and Dennis Shasha,[3] and LRU/K by Pat O'Neil, Betty O'Neil and Gerhard Weikum.[4]
The access sequence for the below example is A B C D E D F.
LRU working
In the above example once A B C D gets installed in the blocks with sequence numbers(Increment 1 for each new Access) and when E is accessed ,it is a miss and it needs to be installed in one of the blocks.According LRU Algorithm,since A has the lowest Rank(A(0)),E will replace A. There is an error in the image where the first line of the second column should be E(4) B(1) C(2) D(3) instead of A(0) B(1) C(2) E(4). 
