## Title
Voter Redistricting

## Slug
voter-redistricting

## Difficulty
Hard

## Description
A politician redraws district lines. Each district elects a candidate from the party (ID) that has the most registered voters in that district.

Mayor Quimby has a collection of $n$ voters, where each voter is represented by an integer ID.

To predict the election outcome, Mayor Quimby must partition these voters into several non-empty districts. Every voter from the original collection must belong to exactly one district. From each district, a "elected official" is extracted. The elected official is defined as the **mode** (most frequent element) of the voters in that district. If a district has multiple voters tied for the most frequent appearance, any one of them can be chosen as the elected official.

Mayor Quimby collects all the extracted elected officials to form a final multiset. Your task is to calculate how many distinct final multisets can be created using this process. Two multisets are considered different if the frequency of any ID differs between them.

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
1. Partition into {1, 2, 2} -> elected official is 2 -> Result {2}.
2. Partition into {1, 2}, {2} -> elected officials 1, 2 or 2, 2 -> Result {1, 2} or {2, 2}. (Wait, if {1, 2} mode can be 1 or 2. If we pick 2, result is {2, 2}).
3. Partition into {1}, {2, 2} -> elected officials 1, 2 -> Result {1, 2}.
4. Partition into {1}, {2}, {2} -> elected officials 1, 2, 2 -> Result {1, 2, 2}.
Total distinct multisets: {2}, {2, 2}, {1, 2}, {1, 2, 2}.

## Input Format
- The first line contains an integer $n$, the number of voters.
- The second line contains $n$ space-separated integers representing the voter IDs.

## Output Format
- Return a single integer representing the number of different multisets of elected officials possible, modulo $998244353$.

## Constraints
- 1 ≤ n ≤ 5000
- 1 ≤ ID ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, math, combinatorics
