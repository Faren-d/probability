# Multinomial coefficients

Let's imagine a scenario where you and eight friends (a total of nine students) want to move into a dorm with three available rooms:

● A double (holds 2 students)

● A triple (holds 3 students)

● A quad (holds 4 students)

The question is: How many different ways can the nine of you be assigned to these rooms?

You might start by thinking:

● First, choose 4 students out of 9 for the quad. This can be done in "9 choose 4" ways (using binomial coefficients).

● Then, choose 3 students out of the remaining 5 for the triple. This can be done in "5 choose 3" ways.

So, the total number of ways seems to be "9 choose 4" multiplied by "5 choose 3."

However, what if you chose the students for the double room first, and then the triple? Would that change the number of possibilities?

This line of thinking leads to the concept of multinomial coefficients, which provide a general way to calculate the number of ways to divide a set of objects into multiple groups of specific sizes.

Just like the dorm room example, multinomial coefficients can also be applied to other scenarios, such as counting the number of possible anagrams of a word with repeated letters.


## Example: Think about the "Mississippi" example to illustrate how multinomial coefficients handle anagrams with repeated letters:

How many different ways can we rearrange these letters to form distinct anagrams?

The word "Mississippi" has 11 letters:

●Four "S"s

●Four "I"s

●Two "P"s

●One "M"


### Solution

Imagine you have 11 empty slots representing the positions in the anagram where you'll place the letters. Instead of focusing on individual letters, consider assigning the groups of letters to these slots. Four "S"s, four "I"s, two "P"s, and one "M".

○ We first choose 4 slots out of 11 for the 'S's. These slots don't have to be together; they can be any 4 slots out of the 11. For instance, we could choose slots 1, 3, 5, and 9.

○ Four slots out of the remaining seven for the "I"s. Again, these can be any 4 slots.

○ Two slots out of the remaining three for the "P"s.

○ The last slot automatically goes to the "M"

○ The multinomial coefficient, (11 choose 4, 4, 2, 1), represents the product of these individual choices:
(11 choose 4) * (7 choose 4) * (3 choose 2) = 34,650

### Important note

- The multinomial coefficient considers all possible combinations of slot assignments for each group of letters, ensuring that we count arrangements with letters both grouped and scattered. In other words, we're choosing slots without any restriction on their order or adjacency. The multinomial coefficient in our example (11 choose 4, 4, 2, 1) considers all possible combinations of slot assignments for each group of letter without being limited to arrangements where the groups of identical letters are clustered together.
