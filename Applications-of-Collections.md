### Applications of Collections

How to calculate the number of ways to choose a collection of objects from a larger set, where the order of selection doesn't matter. This is represented by the binomial coefficient, denoted as "n choose k"(n k), where:

- n is the total number of objects in the pool
- k is the number of objects you want to choose

The formula for calculating this is: (n k) = n! / (k! * (n-k)!)


Here are two examples from the source illustrating this concept:

1. Ordering a pizza with specific toppings: Imagine a pizza place offers 7 meat toppings and 6 veggie toppings. You want a pizza with 2 meat and 2 veggie toppings. To calculate the number of possible pizzas, you would:23
- Calculate the number of ways to choose 2 meat toppings from 7: 7 choose 2, which equals 21.
(7 2) = 7!/2! * 5! = 21
- Calculate the number of ways to choose 2 veggie toppings from 6: 6 choose 2, which equals 15.
(6 2) = 15
Multiply these two numbers to find the total number of possible pizzas: 21 * 15 = 315.

2. Walking routes on a city grid: Imagine you live and work on corners of a rectangular city grid. Your workplace is 3 blocks north and 4 blocks east of your home. To calculate the number of different routes you could walk, you would:456






- Recognize that any route requires 7 moves (3 north and 4 east).
- Think of these moves as a sequence of "N" (north) and "E" (east), like "NEEENNE".
- The problem becomes choosing which 4 of the 7 moves will be "E" (east).
- This is equivalent to 7 choose 4, which equals 35, meaning there are 35 different walking routes.
These examples demonstrate how the binomial coefficient can be used to calculate the number of possible combinations in various scenarios

