## Title
Pilot Co-Pilot

## Slug
pilot-co-pilot

## Difficulty
Easy

## Description
An airline schedules flights. Each flight number ID must have exactly two pilots assigned.

The roster shows a list of pilots, represented by their IDs. For the flight safety, every type of pilot in the list must appear **exactly twice**.

You can perform two types of operations:
1. **Assign**: Add a new pilot of an existing ID (cost: 1).
2. **Dismiss**: Remove an existing pilot from the list (cost: 1).

Your task is to determine the **minimum number of operations** required so that every pilot ID present in the final list has a frequency of exactly 2.

## Examples

### 1

#### Input
5
1 1 1 2 3

#### Output
3

#### Explanation
- ID 1: Count is 3. Dismiss one to make count 2 (Cost 1).
- ID 2: Count is 1. Assign one to make count 2 (Cost 1).
- ID 3: Count is 1. Assign one to make count 2 (Cost 1).
Total cost: 1 + 1 + 1 = 3.

### 2

#### Input
4
10 10 20 20

#### Output
0

#### Explanation
Both ID 10 and ID 20 already appear exactly twice. No operations are needed.

## Input Format
- The first line contains an integer $n$ ($1 \le n \le 10^5$), the number of pilots.
- The second line contains $n$ space-separated integers $a_i$ ($1 \le a_i \le 10^9$), representing the pilot IDs.

## Output Format
- Return a single integer representing the minimum operations required.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ a_i ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
greedy, array, hash-table

