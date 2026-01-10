## Title
Music Note Sequence

## Slug
music-note-sequence

## Difficulty
Medium

## Description
Notes in a melody are played. The melody is 'recognizable' from the start if notes 1 to k have been played.

There is a sequence of $n$ notes indexed from $1$ to $n$. Initially, all notes are **silent**.

You play the notes one by one in a specific order given by an array `sequence`. In the $i$-th step (1-indexed), you play the note at the position `sequence[i-1]`.

A state is called **recognizable** if, after performing $k$ steps, exactly the first $k$ notes (indices $1$ to $k$) are played and all other notes are silent.

Your task is to calculate how many times the system becomes **recognizable** during the entire process.

## Examples

### 1

#### Input
5
3 2 4 1 5

#### Output
2

#### Explanation
- Step 1 (index 3): "__♪__" (Not recognizable)
- Step 2 (index 2): "_♪♪__" (Not recognizable)
- Step 3 (index 4): "_♪♪♪_" (Not recognizable)
- Step 4 (index 1): "♪♪♪♪_" (recognizable: first 4 are played)
- Step 5 (index 5): "♪♪♪♪♪" (recognizable: first 5 are played)
Total recognizable states: 2.

### 2

#### Input
4
4 1 2 3

#### Output
1

#### Explanation
- Step 1 (index 4): "___♪" (Not recognizable)
- Step 2 (index 1): "♪__♪" (Not recognizable)
- Step 3 (index 2): "♪♪_♪" (Not recognizable)
- Step 4 (index 3): "♪♪♪♪" (recognizable)
Total recognizable states: 1.

## Input Format
- The first line contains an integer $n$.
- The second line contains $n$ space-separated integers representing the array `sequence`.

## Output Format
- Return a single integer representing the number of times the state was recognizable.

## Constraints
- 1 ≤ n ≤ 10^4
- `sequence` is a permutation of numbers from $1$ to $n$.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, greedy

## Company
google
