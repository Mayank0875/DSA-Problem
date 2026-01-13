## Title
DNA Gene Splicing

## Slug
dna-gene-splicing

## Difficulty
Medium

## Description
Multiple DNA strands are aligned. Scientists want to cut all strands at a point that disrupts the fewest gene sequences.

There is a DNA sample consisting of $n$ strands. Each strand is composed of several genes, each having a specific length (integers). The total length of every strand is identical.

You need to make a cut from the top to the bottom of the DNA sample that minimizes the number of genes it disrupts.

If the cut passes exactly through the linker region between two genes, it is **not** considered as disrupting a gene. However, you cannot place the cut at the very 5' end or the very 3' end of the DNA sample.

Given the 2D array `structure` containing the lengths of the genes in each strand, return the minimum number of genes disrupted.

## Examples

### 1

#### Input
6
1 2 2 1
3 1 2
1 3 2
2 4
3 1 2
1 3 1 1

#### Output
2

#### Explanation
The total length is 6.
We can make a cut at distance 4 from the 5' end.
- Strand 1: 1+2+2=5 (Disrupt)
- Strand 2: 3+1=4 (Linker)
- Strand 3: 1+3=4 (Linker)
- Strand 4: 2 (Disrupt)
- Strand 5: 3+1=4 (Linker)
- Strand 6: 1+3=4 (Linker)
The cut disrupts strands 1 and 4. Total: 2.

### 2

#### Input
3
1
1
1

#### Output
3

#### Explanation
There are no internal linker regions. Any cut drawn must disrupt all 3 genes.

## Input Format
- The first line contains an integer $n$, the number of strands.
- The next $n$ lines each contain space-separated integers representing the lengths of the genes in that strand.

## Output Format
- Return a single integer representing the minimum number of genes disrupted.

## Constraints
- 1 ≤ n ≤ 10^4
- 1 <= structure[i].length <= 10^4
- The sum of elements in each row is the same.
- 1 <= structure[i][j] <= 2^31 - 1

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table, prefix-sum

