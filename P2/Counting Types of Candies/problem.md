## Title

Counting Types of Candies

## Slug

counting-types-of-candies

## Difficulty

Easy

## Description

After a party, a child has collected a big bag of candies. Each type of candy has a specific numerical code. The bag contains many candies, and there might be several candies of the same type. The child is curious to know how many different kinds of candy they received. You are given a list representing the numerical codes of all the candies in the bag. Calculate how many unique candy types there are.

## Examples

### 1

#### Input

5
[2, 3, 2, 2, 3]

#### Output

2

#### Explanation

The candy codes are 2, 3, 2, 2, 3. The unique codes are 2 and 3. There are 2 distinct candy types.

### 2

#### Input

8
[10, 5, 10, 2, 5, 10, 5, 2]

#### Output

3

#### Explanation

The unique codes are 10, 5, and 2. There are 3 distinct candy types.

## Input Format

- The first line contains an integer n: the total number of candies.
- The second line contains $n$ integers x_1, x_2, ...., x_n: the identification codes of the candies.

## Output Format

- Return a single integer: the count of distinct candy codes.

## Constraints

- 1 ≤ n ≤ 1e5
- 1 ≤ x_i ≤ 1e9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

sorting, set, counting