## Title
Chemical Bonds

## Slug
chemical-bonds

## Difficulty
Easy

## Description
A chemist stabilizes molecules. Each atom type in the solution must bond with exactly one other of its kind (diatomic).

The solution contains a list of atoms, represented by their IDs. For the reaction stability, every type of atom in the list must appear **exactly twice**.

You can perform two types of operations:
1. **Inject**: Add a new atom of an existing ID (cost: 1).
2. **Extract**: Remove an existing atom from the list (cost: 1).

Your task is to determine the **minimum number of operations** required so that every atom ID present in the final list has a frequency of exactly 2.

## Examples

### 1

#### Input
5
1 1 1 2 3

#### Output
3

#### Explanation
- ID 1: Count is 3. Extract one to make count 2 (Cost 1).
- ID 2: Count is 1. Inject one to make count 2 (Cost 1).
- ID 3: Count is 1. Inject one to make count 2 (Cost 1).
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
- The first line contains an integer $n$ ($1 \le n \le 10^5$), the number of atoms.
- The second line contains $n$ space-separated integers $a_i$ ($1 \le a_i \le 10^9$), representing the atom IDs.

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

