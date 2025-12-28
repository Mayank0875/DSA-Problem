## Title
Car Dealership

## Slug
car-dealership

## Difficulty
Medium

## Description
Cars are sold. The Luxury division takes the sports cars, the Mid-range (you) takes the sedans, and Economy takes the compacts.

There are $3n$ cars of varying price available. The distribution follows a strict protocol. In each round, you must select any 3 cars. The parties then claim them based on the following rules:

1. The **Luxury** takes the car with the **maximum** price from the triplet.
2. You, the **Mid-range**, take the car with the **second maximum** price.
3. The **Economy** takes the remaining car (the one with the minimum price).

This process repeats until all cars are distributed. Your goal as the Mid-range is to maximize the total price of the cars you acquire.

Given an array of integers `cars`, where `cars[i]` represents the price of the $i$-th car, return the maximum total price you can obtain.

## Examples

### 1

#### Input
6
2 4 1 2 7 8

#### Output
9

#### Explanation
You have 6 cars. One optimal strategy is:
1. Pick the triplet `(2, 7, 8)`. Luxury takes `8`, you take `7`, Economy takes `2`.
2. Pick the remaining `(1, 2, 4)`. Luxury takes `4`, you take `2`, Economy takes `1`.
Total price = $7 + 2 = 9$.

### 2

#### Input
3
2 4 5

#### Output
4

#### Explanation
There is only one triplet `(2, 4, 5)`. Luxury takes `5`, you take `4`, Economy takes `2`. Total = 4.

## Input Format
- The first line contains a single integer $3n$, the number of cars.
- The second line contains $3n$ space-separated integers representing the `cars` array.

## Output Format
- Return a single integer representing the maximum total price you can collect.

## Constraints
- 1 ≤ cars.length ≤ 10^5
- `cars.length` is divisible by 3.
- 1 ≤ cars[i] ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, sorting, greedy, math
