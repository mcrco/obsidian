**Marco Yang**

I started by implementing the Stack data structure using the built-in Python list. I then tested the Stack data structure by creating an instance in iPython and calling each class function. Everything seemed to work well, so I created the Hanoi class. The only major decision I had to make was how I should represent the pegs, whether it was as a list of three Stacks, three variables, or a dictionary of three Stacks. In the end, I chose the dictionary representation as it allowed me to pass in characters into my disk-moving functions instead of integer indices for arrays or references to the variables.

```
hanoi = Hanoi(initial disks)

# Dictionary implementation (cleanest)
hanoi.move('A', 'B')

# List implementation
hanoi.move(0, 1) # pretty confusing as to what 0 and 1 are

# Three named instances/variables
hanoi.move(hanoi.peg_A, hanoi.peg_B) # ewww!
```

After implementing the move function (no recursion stuff yet), I tested it in an iPython kernel before moving on to the recursion part. I was very confused to see that every time I moved a disk to or from peg B or C, both peg B and C would change. I quickly realized that my constructor for the Stack data structure set the default value for its initial values to the same empty array for every instance.

```
class Stack:
	def __init__(self, initial_arr=[]):
		self.arr = initial_arr
```

I wrote this initially because I wanted to initialize empty Stacks by coding

```
empty_stack = Stack()
```

I had to modify the constructor to 

```
class Stack:
	def __init__(self, initial_arr):
		self.arr = initial_arr
```

and create empty Stacks with the following code:

```
empty_stack = Stack([])
```

After debugging this, the recursion part went smoothly since I have done Tower of Hanoi and similar problems many times before.