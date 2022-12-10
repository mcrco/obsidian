saxophoningR7.1, 2, 4, 7, 8, 15, 16, 19, 21 27

#### 7.1

| a | b | &p | p | 
| --- | --- | --- | ---|
| 1000 | 2000 | &a | 1000 |
| 3000 | 2000 | &a | 3000 |
| 3000 | 2000 | &b | 3000 |
| 6000 | 2000 | &b | 3000 |

#### 7.2

| a | b | p | q | 
| ---- | ---- | ---- | ---- |
| 1000 | 2000 | &a | &b |
| 2000 | 2000 | &a | &b |
| 2000 | 2000 | &b | &b |
| 3000 | 2000 | &b | &b |

#### 7.4

One line 3, he reinitializes p's pointer to a's point, but that's illegal because p is a pointer to an integer, which has a different size compared to q, a double. Line 5 is also illegal because it assignes a pointer without a memory allocation to a value.

#### 7.7

a. {2, 3, 5, 7, 11, 13}
b. 20300
c. 20556
d. 11
e. 11
f. 20556

#### 7.8

a. 41
b. 17
c. 12
d. 0
e. doesn't work

#### 7.15

a. sets p to have a null reference, so it doesn't point anywhere and the program knows that when referencing it
b. sets q to an empty string, so it has a valid reference and value.
c. sets the firts character in a character array to the null character.

#### 7.16

5; it counts the number of tokens separated by strings.

#### 7.19

| legal | illegal|
| --- | --- |
| 1-6, 10-12 | 7-9|

#### 7.21

2: assigning p to 5 is probably wrong because p should point to a memory address.
3: wrong because p doesn't have a proper value cuz the memory address most likely doesn't contain an int
5: s is not a pointer and cannot be used as such
6: cannot delete s because it doesn't point to memory
9: cannot use a like a normral array because it is a pointer
12: q doesn't have memory
15: p refers to same memory address as q, so it is already deleted

#### 7.27 

![[Pasted image 20221208235437.png]]
