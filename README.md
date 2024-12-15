# probability
## Fat Chance: Probability from the Ground Up byedX, HarvardX
```https://learning.edx.org/course/course-v1:HarvardX+FC1x+1T2024/block-v1:HarvardX+FC1x+1T2024+type@sequential+block@b7ea1ff4bf5b4a9b8912e1fabdb6e850/block-v1:HarvardX+FC1x+1T2024+type@vertical+block@90f536d8c7ee4b8dad24e6f779db03b6?_gl=1%2Aklnbwc%2A_gcl_au%2ANzI3ODAwNDg3LjE3MzI2MTQ2MTI.%2A_ga%2AMzIzNTY0NzAzLjE3MzI2MTQ2MTM.%2A_ga_D3KS4KMDT0%2AMTczMjYxNDYxMi4xLjEuMTczMjYxNDcyMC4yNi4wLjA```


## These two examples illustrate what we call the multiplication principle.
#### The number of ways of making a sequence of independent choices: is just the product of the number of choices at each step.

## Factorial notation
### n! : n exclamation mark

## Subtraction principle

The point is that it's sometimes easier to count the objects that don't satisfy the condition, like the vowels, then the objects that do-- the consonants. 

And subtracting off that answer gives the right answer, which is why we call it the subtraction principle.

### Example:

How many numbers between 23 and 283 are not divisible by 5?

Well, by the subtraction principle, we want to calculate the total number of numbers and subtract the ones which are divisible by 5. The total number is 283 minus 22, which is 261 numbers.The ones divisible by 5 run from 25 to 280. And dividing those by 5, you get the numbers between 5 and 56. So our previous method show that there are 56 minus 4 or 52 numbers that are divisible by 5.

First, count the TOTAL number of numbers in the range

Then, count the numbers DIVISIBLE by 5

Subtract the numbers divisible by 5 from the total number

Total number of numbers: Range is from 23 to 283

Total numbers = 283 - 23 + 1 = 261 numbers (We add 1 because we're counting inclusively)

Numbers divisible by 5:

- Smallest number divisible by 5 in this range: 25 -----This means 25 is the 5th number in the sequence of numbers divisible by 5
- Largest number divisible by 5 in this range: 280  -----This means280 is the 56th number in the sequence of numbers divisible by 5

- So the range 5 to 56 represents the INDEX of these numbers in the sequence of numbers divisible by 5, not the actual numbers themselves.
Let's verify:

- 5th number divisible by 5 starts at 25
- 56th number divisible by 5 ends at 280
- Count of numbers: 56 - 5 + 1 = 52 numbers divisible by 5

Final calculation:

- Total numbers: 261
- Numbers divisible by 5: 52
- Numbers NOT divisible by 5: 261 - 52 = 209

## Counting Collections

what are the difference between sequences and collections, and how to calculate the number of possible collections (combinations) of objects from a larger set?

### Sequences vs. Collections:

Sequences are ordered arrangements of objects, while collections are unordered sets of objects.In other words, A collection is different from a sequence, as the objects in a collection are not ordered.
Example: Electing class officers (President, Vice President, etc.) is a sequence, while choosing a committee of students is a collection.

##### Calculating the number of Collections:


Take the example of choosing a committee of 5 students from a class of 15 students.Alice, Bob, Charlie, David, Eve, Frank, Grace, Henry, Ivy, Jack, Kate, Leo, Mike, Nancy, and Oscar.
Let's say we select these 5 students for our committee: Alice, Bob, Charlie, David, and Eve.

The process involves:

- Calculating the number of possible sequences using the multiplication principle: 15 * 14 * 13 * 12 * 11 = 15! / 10!

- But how many ways can we arrange these 5 students?

- 1st position can be filled by ANY of the 5 students
- 2nd position by ANY of the remaining 4
- 3rd position by ANY of the remaining 3
- 4th position by ANY of the remaining 2
- 5th position by the last remaining student

This gives us: 5 × 4 × 3 × 2 × 1 = 5! = 120 different sequences

- Recognizing that each collection of 5 students can be arranged into 5! different sequences.

Setting up an equation: N (number of collections) * 5! = 15! / 10!

Unique collections: Solving for N: N = (15! / 10!) / 5! = 3003

- Important takeaways:

Understanding the distinction between sequences and collections is crucial for accurately counting possibilities.

The multiplication principle is a powerful tool for calculating both sequences and collections.

The formula for calculating the number of collections is derived from understanding the relationship between sequences and collections.

- Imagine you have 15 students and want to choose 5 for a committee. If order matters (sequence), you care WHO is first, second, etc. This gives 15 × 14 × 13 × 12 × 11 possibilities. If order doesn't matter (collection), you just want WHICH 5 students, not their specific order. So each unique group of 5 students can be internally shuffled in 5! (120) different ways.

- By dividing the total sequence count by these internal shuffles (5!), you eliminate all those redundant arrangements that represent the same underlying group.

- Note: Mathematically, division is a form of subtraction. Just like 10 ÷ 2 means "how many groups of 2 can I remove from 10", here we're removing redundant arrangements from the total count.
- The key point: We want to count unique groups, not every possible ordering of those groups.

- For deep understanding, watch: "2.1 Lesson: Counting Collections from the fat chance probability course."

### symmetry of combinations

![n2](https://github.com/user-attachments/assets/4f1ba162-25bc-4cd4-b62c-b85ecc47b42d)

- This states that the binomial coefficient "n choose k"  is equal to "n choose n minus k".

- For example, the number of ways to choose 5 cards from a deck of 52 cards (i.e., 52 choose 5) is the same as the number of ways to choose the 47 cards that are not selected (i.e., 52 choose 47).
The key idea is that the number of ways to choose a collection of k objects from a set of n objects is the same as the number of ways to choose the remaining n-k objects. This relationship is captured in the equation shown in the image.

- 
![n](https://github.com/user-attachments/assets/cbedfe4c-a7b6-4593-8091-3ec8f674dabd)

- This formula means that the number of ways to choose k objects from a set of n objects can be broken down into two cases:

- The number of ways to choose k objects from the n-1 objects, excluding the first one.
- The number of ways to choose k-1 objects from the n-1 objects, excluding the first one.

Let's consider a specific example related to poker hands. The number of 5-card hands that can be dealt from a 52-card deck, 52 choose 5, represents the total number of possible poker hands.

To apply the recursive formula, we can divide the 5-card hands into two groups: those that contain the ace of spades, and those that do not. The number of hands without the ace of spades is 51 choose 5, and the number of hands with the ace of spades is 51 choose 4. Since every 5-card hand either contains the ace of spades or does not, we can add these two values to get the total number of 5-card hands, 52 choose 5.
