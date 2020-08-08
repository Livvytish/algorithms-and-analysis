# Week 1 - Algorithms analysis and fundemental data structures

## 1. What is an algorithm and what are its characteristics? Are algorithms language-specific? Explain the derivation of the term “algorithm.”

- **What is an algorithm?**
  - Sequence of unambiguous instructions
  - Solves a problem
  - Obtains required output
  - Based on any legitimate input in a finite amount of time

- Algorithms are **not** language specific

- Comes from the latinisation of the name of some Arabic man :)

## 2. Given that the official purpose of the U.S. patent system is the promotion of the “useful arts,” do you think algorithms are patentable in this scountry? Should they be?

Depends on the perspective you look at it from!

## 3. 

### a. Write down the steps for installing a television set in your home with the precision required from an algorithm’s description.

1. Place TV on cabinet
2. Plug chord into back of TV.
3. Plug plug into wall
4. Turn plug on
5. Turn TV on

### b. Write down the steps for preparing tea with the precision required by an algorithm.

1. Get kettle
2. Open spout
3. Fill kettle with water for one cup
4. Turn off tap
5. Put kettle on gas top
6. Light flame
7. Waiting for water to boil
8. Turn off gas
9. Get cup
10. Get teabag
11. Put teabag in cup
12. Fill cup with water from kettle
13. Let brew for 3 minutes
14. Retrieve teabag
15. Get milk
16. Pour 10ml milk

## 4. Write an algorithm for sorting integer numbers in ascending order using any sorting technique. For example, the unsorted numbers are 23, 45, 12, 37, 11, 56 and the sorted numbers in ascending order are 11, 12, 23, 37, 45, 56.

```
numbers = [23, 45, 12, 37, 11, 56]

# Bubble sort - swap adjacent numbers

for(i=0 i<numbers.length-1 i++) 
{
numbers[i] < numbers[i+1]? do nothing
else swap
swapcount++
}

repeat until swapcount = 0
```

## 5. Design an algorithm to find the sorted list from two sorted lists of numbers. For example, for the lists 2, 5, 7, 12, 13, 24 and 1, 6, 15, 17, 35, the output should be 1, 2, 5, 6, 7, 12, 13, 15, 17, 24, 35. What is the maximum number of comparisons your algorithm makes if the lengths of the two given lists are m and n, respectively?

```
a = [2, 5, 7, 12, 13, 24]
b = [1, 6, 15, 17, 35]
c = []

# Bubble sort - swap adjacent numbers

whilst c.length < (a.length+b.length)
{
a[i] < b[i]? do nothing
else swap
swapcount++
}

repeat until swapcount = 0
```


- Maximum number of comparisons is `n x m`

## 6. a. Find gcd(31415, 14142) by applying Euclid’s algorithm.
b. Estimate how many times faster it will be to find gcd(31415, 14142) by Euclid’s algorithm compared with the algorithm based on checking con- secutive integers from min{m, n} down to gcd(m, n).

## 7. Prove the equality gcd(m, n) = gcd(n, m mod n) for every pair of positive integers m and n.

## 8. What does Euclid’s algorithm do for a pair of integers in which the first is smaller than the second? What is the maximum number of times this can happen during the algorithm’s execution on such an input?

## 9. a. b. What is the maximum number of divisions made by Euclid’s algorithm
What is the minimum number of divisions made by Euclid’s algorithm among all inputs 1 ≤ m, n ≤ 10?

## 10. a.
among all inputs 1 ≤ m, n ≤ 10?
Euclid’s algorithm, as presented in Euclid’s treatise, uses subtractions rather than integer divisions. Write pseudocode for this version of Euclid’s algorithm.
b. PUZZLE Euclid’s game (see [Bog]) starts with two unequal positive integers on the board. Two players move in turn. On each move, a player has to write on the board a positive number equal to the difference of two numbers already on the board; this number must be new, i.e., different from all the numbers already on the board. The player who cannot move loses the game. Should you choose to move first or second in this game?

## 11. The extended Euclid’s algorithm determines not only the greatest common divisor d of two positive integers m and n but also integers (not necessarily positive) x and y, such that mx + ny = d. a. LookupadescriptionoftheextendedEuclid’salgorithm(see,e.g.,[KnuI,
p. 13]) and implement it in the language of your choice. b. ModifyyourprogramtofindintegersolutionstotheDiophantineequation
ax + by = c with any set of integer coefficients a, b, and c.

## PUZZLE 12.	Locker doors	There are n lockers in a hallway, numbered sequentially from 1 to n. Initially, all the locker doors are closed. You make n passes by the lockers, each time starting with locker #1. On the ith pass, i = 1, 2, . . . , n, you toggle the door of every ith locker: if the door is closed, you open it; if it is open, you close it. After the last pass, which locker doors are open and which are closed? How many of them are open?