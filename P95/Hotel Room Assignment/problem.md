## Title
Hotel Room Assignment

## Slug
hotel-room-assignment

## Difficulty
Hard

## Description
Guests are assigned to floors. The demographic of a floor is the most common guest type ID.

The Concierge has a collection of $n$ guests, where each guest is represented by an integer ID.

To optimize service, The Concierge must partition these guests into several non-empty floors. Every guest from the original collection must belong to exactly one floor. From each floor, a "demographic" is extracted. The demographic is defined as the **mode** (most frequent element) of the guests in that floor. If a floor has multiple guests tied for the most frequent appearance, any one of them can be chosen as the demographic.

The Concierge collects all the extracted demographics to form a final multiset. Your task is to calculate how many distinct final multisets can be created using this process. Two multisets are considered different if the frequency of any ID differs between them.

## Examples

### 1

#### Input
3
1 2 3

#### Output
7

#### Explanation
Any non-empty subset of {1, 2, 3} can be achieved, for a total of 7 multisets.

### 2

#### Input
3
1 2 2

#### Output
4

#### Explanation
We can generate 4 different multisets:
1. Partition into {1, 2, 2} -> demographic is 2 -> Result {2}.
2. Partition into {1, 2}, {2} -> demographics 1, 2 or 2, 2 -> Result {1, 2} or {2, 2}. (Wait, if {1, 2} mode can be 1 or 2. If we pick 2, result is {2, 2}).
3. Partition into {1}, {2, 2} -> demographics 1, 2 -> Result {1, 2}.
4. Partition into {1}, {2}, {2} -> demographics 1, 2, 2 -> Result {1, 2, 2}.
Total distinct multisets: {2}, {2, 2}, {1, 2}, {1, 2, 2}.

## Input Format
- The first line contains an integer $n$, the number of guests.
- The second line contains $n$ space-separated integers representing the guest IDs.

## Output Format
- Return a single integer representing the number of different multisets of demographics possible, modulo $998244353$.

## Constraints
- 1 ≤ n ≤ 5000
- 1 ≤ ID ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, math, combinatorics
