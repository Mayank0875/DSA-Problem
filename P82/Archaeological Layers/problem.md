## Title
Archaeological Layers

## Slug
archaeological-layers

## Difficulty
Easy

## Description
An excavator finds n artifacts. They want to display a timeline of increasing technological complexity.

You have complexity scores for n artifacts found in order.
A technological progression consists of artifacts where complexity is strictly higher than the previous one.

You must curate the exhibit to find the longest possible progression timeline. You can skip any number of artifacts to form the sequence, but you must maintain the original discovery order of the selected artifacts. Calculate the maximum number of artifacts that can form such a sequence.

## Examples

### 1

#### Input
8
7 3 5 3 6 2 9 8

#### Output
4

#### Explanation
The input contains: [7, 3, 5, 3, 6, 2, 9, 8]. The longest progression timelines (strictly increasing) include:
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
Since the values are strictly decreasing, we can pick at most 1 artifact.

## Input Format
- The first line contains an integer n: the number of artifacts.
- The second line contains n integers x_1, x_2 ... x_n: the complexity of each artifact in order.

## Output Format
- Return one integer: the length of the longest valid progression timeline.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, dynamic-programming, greedy
