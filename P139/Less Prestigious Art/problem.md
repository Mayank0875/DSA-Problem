## Title
Less Prestigious Art

## Slug
less-prestigious-art

## Difficulty
Medium

## Description
A gallery curates paintings.

You have a list of $n$ paintings. Each painting has two main properties: **age** and **artist rank**. You are given a 2D integer array `properties` where `properties[i] = [age_i, artist rank_i]` represents the attributes of the $i$-th painting.

A painting is considered **less prestigious** if there exists another painting that has **both** strictly greater age and strictly greater artist rank.

More formally, the $i$-th painting is less prestigious if there exists an index $j$ such that `age_j > age_i` and `artist rank_j > artist rank_i`.

Your task is to return the number of less prestigious paintings.

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
No painting has strictly greater age and artist rank than another.

### 2

#### Input
2
2 2
3 3

#### Output
1

#### Explanation
The first painting (2, 2) is less prestigious because the second painting (3, 3) has strictly greater age and artist rank.

## Input Format
- The first line contains an integer $n$, the number of paintings.
- The next $n$ lines each contain two space-separated integers, representing the age and artist rank of a painting.

## Output Format
- Return a single integer representing the number of less prestigious paintings.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ age, artist rank ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, greedy, sorting
