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