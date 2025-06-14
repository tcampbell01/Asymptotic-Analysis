
==Discrete probability== is concerned with experiments in which the sample space is a finite or countably infinite set. Almost all of the experiments analyzed in this material have finite sample spaces. A set is ==countably infinite if there is a one-to-one correspondence between the elements of the set and the integers.== An infinite set that is not countably infinite is uncountably infinite. A formal discussion of the different kinds of infinity is beyond the scope of this material, but the following examples give an intuitive feel for the difference between countably infinite and uncountably infinite sets.

The probability distribution in which every outcome has the same probability is called the uniform distribution.

P(A U B) = P(A) + P(B) - p(A interset B)

1/4 + 1/4 - 1/8 = 

3 flips of a coin: 
HHH
HHT
HTT
TTT
TTH
THH
HTH
THT

What is the probability that the first two flips are heads or the last two flips are heads

B1 R1
B1 R2 * *
B1 R3
B1 R4
B1 R5
B1 R6

B2 R1
B2 R2
B2 R3 * *
B2 R4
B2 R5
B2 R6

B3 R1
B3 R2
B3 R3
B3 R4 **
B3 R5
B3 R6

B4 R1
B4 R2
B4 R3
B4 R4
B4 R5* 
B4 R6

B5 R1
B5 R2
B5 R3
B5 R4
B5 R5 
B5 R6* 

B6 R1
B6 R2
B6 R3
B6 R4
B6 R5
B6 R6

The complement of an event: The probability that an event doesn't happen can be easier to determine than the probability that the event does happen.

Conditional Probability: 
p(E intersect F)/p(F)

Two events are independent if conditioning on one event does not change the probability of the other event. A formal description in terms of probabilities is given below:

p(F intersect E) = p(F) * p(E)

2/7 * 5/7 = 10/49


Probability: 

|                                                                  |                     |                                                                 |
| ---------------------------------------------------------------- | ------------------- | --------------------------------------------------------------- |
| **‘Event is hard to count directly’**                            | ✅ Often             | Complement may be shorter than listing all favorable outcomes   |
| **‘Exactly k items’ (e.g., exactly one pair)**                   | ❌ No                | Count exactly how many satisfy the given value of k             |
| **‘None of’ (e.g., no hearts in hand)**                          | ✅ Yes               | Count total hands with none of the type and subtract from total |
| **Situation / Clue in Problem**                                  | **Use Complement?** | **How to Approach**                                             |
| **‘Not all’ (e.g., not all dice match)**                         | ✅ Yes               | Same as ‘at least one not…’ so use complement                   |
| **‘At most’ (e.g., at most two red cards)**                      | ✅ Yes               | Use 1 - P(more than the allowed number)                         |
| **‘At least one’ (e.g., at least one club, at least one match)** | ✅ Yes               | Use 1 - P(none of the desired item)                             |
| **‘Specific type of hand’ (e.g., full house, flush)**            | ❌ No                | Use direct combinatorics (choose ranks, suits, etc.)            |
| **‘Total - unwanted cases is easier’**                           | ✅ Definitely        | Use: P(A) = 1 - P(not A)                                        |
