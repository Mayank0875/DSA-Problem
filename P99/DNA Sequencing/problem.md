## Title
DNA Sequencing

## Slug
dna-sequencing

## Difficulty
Hard

## Description
Scientists select gene markers. Markers are chemically linked to successors.

Dr. Helix and Dr. Strand are playing a strategic game using a gene chain $p$ of length $n$. The game starts with a sequence stability of 0.

The players take turns, with Dr. Helix moving first. On each turn, a player chooses an integer $x$ from the gene chain that has not been chosen before.
- If it is Dr. Helix's turn, the chosen value $x$ is **added** to the sequence stability.
- If it is Dr. Strand's turn, the chosen value $x$ is **subtracted** from the sequence stability.

The rules for choosing $x$ are:
1. On the very first move of the game, Dr. Helix may choose **any** unselected gene from the gene chain.
2. On every move after the first:
   - Let $m$ be the index of the gene chosen in the previous move (that is, the previous player chose $p[m]$).
   - If the value $p[m]$ has not yet been chosen, the current player **must** choose $p[m]$.
   - If $p[m]$ has already been chosen, the current player may choose **any** unselected gene.

The game continues until all genes of the gene chain have been chosen.

Dr. Helix plays optimally to **maximize** the final sequence stability, while Dr. Strand plays optimally to **minimize** it.

Your task is to compute the final sequence stability assuming both players play optimally.

## Examples

### 1

#### Input
3
2 3 1

#### Output
4

#### Explanation
Final sequence stability is 4.

### 2

#### Input
2
2 1

#### Output
1

#### Explanation
Final sequence stability is 1.

## Input Format
- The first line contains an integer $n$ (length of gene chain).
- The second line contains $n$ space-separated integers $p_1, \dots, p_n$.

## Output Format
- Return one integer: the final sequence stability on a new line.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ p_i ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
greedy, graph, combinatorics
