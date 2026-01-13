## Title
Weaker Generators

## Slug
weaker-generators

## Difficulty
Medium

## Description
An electrician tests power generators.

You have a list of $n$ generators. Each generator has two main properties: **voltage output** and **amperage**. You are given a 2D integer array `properties` where `properties[i] = [voltage output_i, amperage_i]` represents the attributes of the $i$-th generator.

A generator is considered **weaker** if there exists another generator that has **both** strictly greater voltage output and strictly greater amperage.

More formally, the $i$-th generator is weaker if there exists an index $j$ such that `voltage output_j > voltage output_i` and `amperage_j > amperage_i`.

Your task is to return the number of weaker generators.

## Examples

### 1

#### Input
3
5 5
6 3
3 6

#### Output
0

#### Explanation
No generator has strictly greater voltage output and amperage than another.

### 2

#### Input
2
2 2
3 3

#### Output
1

#### Explanation
The first generator (2, 2) is weaker because the second generator (3, 3) has strictly greater voltage output and amperage.

## Input Format
- The first line contains an integer $n$, the number of generators.
- The next $n$ lines each contain two space-separated integers, representing the voltage output and amperage of a generator.

## Output Format
- Return a single integer representing the number of weaker generators.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ voltage output, amperage ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, greedy, sorting
