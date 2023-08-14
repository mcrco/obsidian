**Marco Yang**

After reading the problem statement, I tried to quickly get a working program creating 2 lists in the main function to keep track of the current states and the new states and 2 helper functions: one to print an array of states as a binary string and one to update the new states list given the current states and new states lists. To simulate each generation, I put updated the new states, printed the new states, and set the current states to the new states for the next generation inside a loop.

```
# First approach pseudocode

update:
	modifies new_states
 
print:
	prints new_states

main:
	initialize curr_states, new_states
	for every generation:
		update
		print
		curr_states = new_states
```

Upon running the code with some test cases, I got a bunch of strings of just 0's after a few generations. I quickly realized that I was  ```curr_states``` to ```new_states```, meaning my update function was modifying both lists: a rookie pass-by-reference vs pass-by-value mistake, so I replaced my update function with a function that returns a fresh array of new cell states each call.

```
# Final approach pseudocode

get_new_states:
	create and return new_states
 
print:
	prints curr_states

main:
	initialize curr_states
	for every generation:
		curr_states = get_new_states
		print
```

I also cleaned up my code by storing the rules as an integer array and not a boolean array so the update code goes from an ```if rule[sum]``` statement to a simple ```new_state = rule[sum]```.