## Title
Magical Spell Weaving

## Slug
magical-spell-weaving

## Difficulty
Medium

## Description
A mage is weaving a spell from a sequence of runes. The runes must be grouped into stanzas to stabilize the magic.

Merlin is working with a sequence of $n$ runes, where the $i$-th rune has a value of $a_i$.

Merlin needs to create a **spell structure**. A spell structure involves dividing the sequence of $n$ runes into one or more contiguous stanzas such that every rune belongs to exactly one stanza.

For a specific spell structure, the **resonance frequency** is calculated as follows:
1. Calculate the sum of values for each stanza in the partition.
2. The resonance frequency is the bitwise XOR sum of these stanza sums.

Your task is to calculate the bitwise XOR sum of the resonance frequency values of **all possible spell structures** of the sequence.

## Examples

### 1

#### Input
1
1

#### Output
1

#### Explanation
Total XOR sum: 1.

### 2

#### Input
2
1 2

#### Output
0

#### Explanation
Partition {1}, {2}: Group sums are 1, 2. XOR sum = 1 ^ 2 = 3.
Partition {1, 2}: Group sum is 3. XOR sum = 3.
Total Result = 3 ^ 3 = 0.

## Input Format
- The first line contains a single integer $n$ — the length of the sequence.
- The second line contains $n$ space-separated integers $a_1, a_2, \dots, a_n$.

## Output Format
- Return a single integer representing the total XOR sum of resonance frequencys of all possible partitions.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ a_i ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming, array
