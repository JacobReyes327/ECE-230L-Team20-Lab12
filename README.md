# Number Theory: Addition

In this lab, you’ve learned about One Hot and Binary state machines and how to build them.

## Rubric

| Item | Description | Value |
| ---- | ----------- | ----- |
| Summary Answers | Your writings about what you learned in this lab. | 25% |
| Question 1 | Your answers to the question | 25% |
| Question 2 | Your answers to the question | 25% |
| Question 3 | Your answers to the question | 25% |

## Lab Questions

## Lab summary

This lab involved building 2 forms of a basic state machine. The One Hot state machine has a D-FlipFlop for every state, meaning there is only one FlipFlop asserted at a time. Using a state machine diagram, the logic of each state can be isolated. Binary implementation has as many D-FlipFlops as represented in binary. For example, 5 states would require 3 bits, or 3 FlipFlops. Using K-maps, the inputs and outputs of the state machine can be reduced to the number of bits needed.


### Compare and contrast One Hot and Binary encodings
Well, for one, One Hot encoding requires a number of bits equal to the number of states possible in the state machine, whereas a binary encoding only requires 2^n number of bits, where n is the number of states. On the other hand, the logic behind One Hot encoding is rather simple when compared to the logic of binary encodings.

### Which method did your team find easier, and why?
We definitly found one hot encoding easier because finding out which state comes next was much simpler, and we could simply route the output of each D-flip-flop into some or gates along with the proper w input into an and gate. Our binary failed many times do to small logic errors in my (Jacob's) k-maps, which were very difficult to find/ apparently impossible to find for me.

### In what conditions would you have to use one over the other? Think about resource utilization on the FPGA.
If you had many states, you would probably want to use binary encoding, because otherwise you may not have enough led's (in our case) or enough flip-flops (in a more official lab case). Basically just saving on physical space would be the reason to use binary over one-hot.
