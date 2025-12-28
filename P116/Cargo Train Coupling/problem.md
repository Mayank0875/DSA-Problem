## Title
Cargo Train Coupling

## Slug
cargo-train-coupling

## Difficulty
Medium

## Description
A yardmaster manages train cars that have specific connector types. Each car has a front connector size and a rear connector size.

You have a list of train cars, each defined by a front connector and an rear connector, represented as a pair `[front, rear]`.

To couple two cars, the rear connector of the first must be smaller than the front connector of the second to fit inside the mechanism. Specifically, to transition from car `[a, b]` to a subsequent car `[c, d]`, the rear of the first car must be **strictly less than** the front of the second car (i.e., `b < c`).

You can select cars in any order you like to form a valid train. Your goal is to determine the maximum number of cars that can be included in a single train.

## Examples

### 1

#### Input
3
1 2
2 3
3 4

#### Output
2

#### Explanation
The longest train is `[1, 2] -> [3, 4]`. You cannot include `[2, 3]` because `2` (end of first) is not strictly less than `2` (start of second).

### 2

#### Input
3
1 2
7 8
4 5

#### Output
3

#### Explanation
The cars can be reordered to form the train `[1, 2] -> [4, 5] -> [7, 8]`. All transitions satisfy `end < start`.

## Input Format
- The first line contains an integer `n`, the number of available cars.
- The next `n` lines each contain two integers, representing the `front` and `rear` of an car.

## Output Format
- Return a single integer representing the maximum length of the train.

## Constraints
- 1 ≤ n ≤ 1000
- -1000 ≤ front < rear ≤ 1000

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy, sorting
