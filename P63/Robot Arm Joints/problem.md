## Title
Robot Arm Joints

## Slug
robot-arm-joints

## Difficulty
Easy

## Description
A robotic arm has $n$ segments. There are 5 types of joints, rated by flexibility. The arm is constructed such that flexibility never decreases from the base to the tip. How many arm designs are valid?

## Examples

### 1

#### Input
1

#### Output
5

#### Explanation
There are 5 valid sequences of length 1.

### 2

#### Input
2

#### Output
15

#### Explanation
There are 15 valid sorted sequences of length 2 (e.g., aa, ae, ai, ao, au, ee, etc.).

## Input Format
- The input consists of a single integer n, representing the required length/quantity.

## Output Format
- Return a single integer representing the total number of valid sorted sequences.

## Constraints
- 1 ≤ n ≤ 50

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, math
