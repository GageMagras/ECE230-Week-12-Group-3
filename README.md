# Finite State Machines

# Group 3: Randy Bauer, Gage Magras

In this lab, you’ve learned about One Hot and Binary state machines and how to build them.

## Rubric

| Item | Description | Value |
| ---- | ----------- | ----- |
| Summary Answers | Your writings about what you learned in this lab. | 25% |
| Question 1 | Your answers to the question | 25% |
| Question 2 | Your answers to the question | 25% |
| Question 3 | Your answers to the question | 25% |

## Lab Questions

Summary here

### Compare and contrast One Hot and Binary encodings

A One Hot implementation requires that we hook up each D flip-flop to an LED on the board which severely limits the number of states that we can manage. This also means that we have to use more D flip-flops than with Binary encoding. With Binary encoding, each bit is managed by a flip-flop which allows us to have more states than the One Hot implementation. This does means there can be a certain number of invalid states since adding one more bit for the Binary finite state machine 'allocates' more room than is needed.

### Which method did your team find easier, and why?

Randy liked the One Hot method because k maps suck and the D flip-flops seemed manageable for state machine of this size. Gage preferred the Binary implementation for its expandability.

### In what conditions would you have to use one over the other? Think about resource utilization on the FPGA.

If we have a limited number of D flip-flops to work with, a Binary implementation is better since we have a limited number D flip-flops and/or programmable features on the board. If you want to make a smaller state machine, the One Hot method is quick to implement and easy to understand.
