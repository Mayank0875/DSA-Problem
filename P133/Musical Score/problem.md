## Title
Musical Score

## Slug
musical-score

## Difficulty
Medium

## Description
Notes are placed on a staff. A vertical line is drawn that intersects the fewest note heads.

There is a score consisting of $n$ staves. Each staff is composed of several notes, each having a specific duration (integers). The total duration of every staff is identical.

You need to draw a measure line from the top to the bottom of the score that minimizes the number of notes it intersects.

If the measure line passes exactly through the rest between two notes, it is **not** considered as intersecting a note. However, you cannot place the measure line at the very start or the very end of the score.

Given the 2D array `structure` containing the durations of the notes in each staff, return the minimum number of notes intersected.

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
The total duration is 6.
We can draw a measure line at distance 4 from the start.
- Staff 1: 1+2+2=5 (Intersect)
- Staff 2: 3+1=4 (Rest)
- Staff 3: 1+3=4 (Rest)
- Staff 4: 2 (Intersect)
- Staff 5: 3+1=4 (Rest)
- Staff 6: 1+3=4 (Rest)
The measure line intersects staves 1 and 4. Total: 2.

### 2

#### Input
3
1
1
1

#### Output
3

#### Explanation
There are no internal rests. Any measure line drawn must intersect all 3 notes.

## Input Format
- The first line contains an integer $n$, the number of staves.
- The next $n$ lines each contain space-separated integers representing the durations of the notes in that staff.

## Output Format
- Return a single integer representing the minimum number of notes intersected.

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

