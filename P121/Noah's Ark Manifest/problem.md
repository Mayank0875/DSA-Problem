## Title
Noah's Ark Manifest

## Slug
noahs-ark-manifest

## Difficulty
Easy

## Description
Noah is preparing the Ark. To save the animals, he needs exactly two of every species identified by their Species ID.

You have a list of animals, represented by their IDs. For the voyage to succeed, every type of animal in the list must appear **exactly twice**.

You can perform two types of operations:
1. **Rescue**: Add a new animal of an existing ID (cost: 1).
2. **Release**: Remove an existing animal from the list (cost: 1).

Your task is to determine the **minimum number of operations** required so that every animal ID present in the final list has a frequency of exactly 2.

## Examples

### 1

#### Input
5
1 1 1 2 3

#### Output
3

#### Explanation
- ID 1: Count is 3. Release one to make count 2 (Cost 1).
- ID 2: Count is 1. Rescue one to make count 2 (Cost 1).
- ID 3: Count is 1. Rescue one to make count 2 (Cost 1).
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
- The first line contains an integer $n$ ($1 \le n \le 10^5$), the number of animals.
- The second line contains $n$ space-separated integers $a_i$ ($1 \le a_i \le 10^9$), representing the animal IDs.

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

