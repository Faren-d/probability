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











