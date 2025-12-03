## Title
DNA Strand Cross-Link

## Slug
dna-strand-cross-link

## Difficulty
Medium

## Description
Biologists are modeling artificial cross-links between two synthetic DNA strands to ensure stability.

Two parallel strands, Helix 1 and Helix 2, each contain n nucleotides arranged in a line.
Helix 1 has an array `a` representing the binding energy of each nucleotide.
Helix 2 has an array `b` representing the binding energy of each nucleotide.

Inside each strand, adjacent nucleotides are already connected by internal sugar-phosphate backbones.

You must establish inter-strand hydrogen bonds connecting some nucleotides of Helix 1 to some nucleotides of Helix 2.

The cost to create a bond between nucleotide i of Helix 1 and nucleotide j of Helix 2 is:
absolute value of (a[i] - b[j]).

**Fault-tolerance requirement:**
The final network must remain fully connected even if any single nucleotide is removed (from either Helix 1 or Helix 2).
If one nucleotide fails and disappears along with all its connections, the remaining nucleotides must still form a single connected network.

Your task is to calculate the minimum total cost required to build such a set of connections.

## Examples

### 1

#### Input
3
1 10 1
20 4 25

#### Output
31

#### Explanation
It's optimal to connect four pairs of nucleotides:
1. nucleotide 1 from Helix 1 with nucleotide 2 from Helix 2: cost |1-4| = 3.
2. nucleotide 3 from Helix 1 with nucleotide 2 from Helix 2: cost |1-4| = 3.
3. nucleotide 2 from Helix 1 with nucleotide 1 from Helix 2: cost |10-20| = 10.
4. nucleotide 2 from Helix 1 with nucleotide 3 from Helix 2: cost |10-25| = 15.
Total cost: 3 + 3 + 10 + 15 = 31.

### 2

#### Input
4
1 1 1 1
1000000000 1000000000 1000000000 1000000000

#### Output
1999999998

#### Explanation
It is optimal to connect the first nucleotide of Helix 1 with the first of Helix 2, and the last nucleotide of Helix 1 with the last of Helix 2, satisfying the connectivity conditions efficiently given the values.

## Input Format
- The first line contains an integer n, the number of nucleotides in each strand.
- The second line contains n integers representing the binding energys of Helix 1.
- The third line contains n integers representing the binding energys of Helix 2.

## Output Format
- Return a single integer representing the minimum total cost to make the network fault-tolerant.

## Constraints
- 3 ≤ n ≤ 10^5
- 1 ≤ a[i], b[i] ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, greedy, math
