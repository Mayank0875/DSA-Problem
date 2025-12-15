## Title
Traffic Speed Monitor

## Slug
traffic-speed-monitor

## Difficulty
Easy

## Description
A radar tracks n cars. It looks for a convoy speeding up, where each car is strictly faster than the one ahead.

You have speeds for n cars.
A speeding convoy consists of cars where speed is strictly higher than the previous car.

You must monitor traffic to find the longest possible speeding convoy. You can skip any number of cars to form the sequence, but you must maintain the original road order order of the selected cars. Calculate the maximum number of cars that can form such a sequence.

## Examples

### 1

#### Input
8
7 3 5 3 6 2 9 8

#### Output
4

#### Explanation
The input contains: [7, 3, 5, 3, 6, 2, 9, 8]. The longest speeding convoys (strictly increasing) include:
3, 5, 6, 9
3, 5, 6, 8
The length of these sequences is 4.

### 2

#### Input
5
5 4 3 2 1

#### Output
1

#### Explanation
Since the values are strictly decreasing, we can pick at most 1 car.

## Input Format
- The first line contains an integer n: the number of cars.
- The second line contains n integers x_1, x_2 ... x_n: the speed of each car in order.

## Output Format
- Return one integer: the length of the longest valid speeding convoy.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, dynamic-programming, greedy
