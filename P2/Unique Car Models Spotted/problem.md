## Title

Unique Car Models Spotted

## Slug

unique-car-models-spotted

## Difficulty

Easy

## Description

A car enthusiast is keeping track of different car models they see on the road. Each car model is identified by a unique numerical code. During their observation period, they might spot the same model multiple times. They want to find out the total number of distinct car models encountered. You are given the list of model codes for every car spotted. Determine the count of unique car model codes.

## Examples

### 1

#### Input

5
[2, 3, 2, 2, 3]

#### Output

2

#### Explanation

The model codes spotted are 2, 3, 2, 2, 3. The unique codes are 2 and 3. The enthusiast saw 2 distinct car models.

### 2

#### Input

8
[10, 5, 10, 2, 5, 10, 5, 2]

#### Output

3

#### Explanation

The unique codes are 10, 5, and 2. The enthusiast saw 3 distinct car models.

## Input Format

- The first line contains an integer n: the total number of cars spotted.
- The second line contains $n$ integers x_1, x_2, ...., x_n: the car model identification codes.

## Output Format

- Return a single integer: the count of distinct model codes.

## Constraints

- 1 ≤ n ≤ 1e5
- 1 ≤ x_i ≤ 1e9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

sorting, set, counting