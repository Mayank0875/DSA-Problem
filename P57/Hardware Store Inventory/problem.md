## Title
Hardware Store Inventory

## Slug
hardware-store-inventory

## Difficulty
Easy

## Description
A hardware store has a bin of mixed screws, nuts, and bolts (characters). Customers submit orders for specific assembly kits. An order can be fulfilled if the bin contains all the required parts. Calculate the total number of parts sold from all fulfillable orders.

## Examples

### 1

#### Input
4
cat bt hat tree
atach

#### Output
6

#### Explanation
The items that can be formed are "cat" and "hat".
"cat" requires 'c', 'a', 't'. The supply "atach" has all of these.
"hat" requires 'h', 'a', 't'. The supply "atach" has all of these.
"bt" requires 'b', which is missing.
"tree" requires 'r' and 'e', which are missing.
Total value = length("cat") + length("hat") = 3 + 3 = 6.

### 2

#### Input
3
hello world code
welldonehoneyr

#### Output
10

#### Explanation
We can form "hello" and "world".
Total value = 5 + 5 = 10.

## Input Format
- The first line contains an integer n, the number of target items.
- The second line contains n space-separated strings representing the `targets`.
- The third line contains a single string representing the `supply` or `inventory`.

## Output Format
- Return a single integer representing the sum of lengths of all formable items.

## Constraints
- 1 ≤ n ≤ 1000
- 1 ≤ targets[i].length, supply.length ≤ 100
- All strings consist of lowercase English letters.

## Time Limit
1 second

## Memory Limit
256 MB

## Tags
string, hash-table
