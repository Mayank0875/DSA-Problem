## Title

Applejack's Sorting Magic

## Slug

applejacks-sorting-magic

## Difficulty

Medium

## Description

Fluttershy and her friends are at Sweet Apple Acres helping Applejack harvest apples. However, some strange magic has caused the apples to behave unpredictably, flying out of baskets and arranging themselves in odd patterns.

To restore order, Applejack needs to sort the apples based on their type. We can represent the row of apples as a binary string $s$ of length $n$, consisting of '0's (Red Delicious) and '1's (Granny Smith). A string is considered **sorted** if all '0's appear before all '1's (e.g., "000111" is sorted, but "101" is not).

You possess a specific magical maneuver to help sort them. In one operation, you can:
1. Choose any substring of $s$.
2. Choose a positive integer $k$.
3. Cyclically shift the chosen substring to the left by $k$ positions.

For example, shifting the substring `1011` of string `0101100` by 2 positions results in `0111000`.

Your task is to calculate the **minimum number of operations** required to make the string $s$ sorted.

## Examples

### 1

#### Input

01010101

#### Output

3

#### Explanation

We need to move the 0s that appear after 1s.
One possible sequence of operations:
Substring 10 at index 1: shift 10 → 01
String becomes: 00110101
Substring 10 at index 4: shift 10 → 01
String becomes: 00101101
Substring 10 at index 6: shift 10 → 01
String becomes: 00101011
Note: The optimal strategy often moves blocks of zeros together.
The logic in the solution computes the minimum number of operations directly, without simulating every swap.
    
### 2

#### Input

11001010001

#### Output

3

#### Explanation

There are three distinct groups of '0's that appear after the first '1'.
The group 00 at indices 2-3.
The group 0 at index 5.
The group 000 at indices 7-9. Each group requires one operation to be moved to the correct position relative to the '1's preceding it.
  

## Input Format  

- The first line contains a single string s consisting only of characters '0' and '1'.

## Output Format  

- Return a single integer representing the minimum number of operations required.
  

## Constraints  

- 1 ≤ s.length ≤ 1e5

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

string, greedy