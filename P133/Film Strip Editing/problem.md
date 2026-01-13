## Title
Film Strip Editing

## Slug
film-strip-editing

## Difficulty
Medium

## Description
Stacked film reels have scenes. You want to cut the reels where the fewest scenes are active (during scene changes).

There is a archive consisting of $n$ reels. Each reel is composed of several scenes, each having a specific duration (integers). The total duration of every reel is identical.

You need to make a cut from the start to the end of the archive that minimizes the number of scenes it interrupts.

If the cut passes exactly through the change between two scenes, it is **not** considered as interrupting a scene. However, you cannot place the cut at the very start or the very end of the archive.

Given the 2D array `structure` containing the durations of the scenes in each reel, return the minimum number of scenes interrupted.

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
We can make a cut at distance 4 from the start.
- Reel 1: 1+2+2=5 (Interrupt)
- Reel 2: 3+1=4 (Change)
- Reel 3: 1+3=4 (Change)
- Reel 4: 2 (Interrupt)
- Reel 5: 3+1=4 (Change)
- Reel 6: 1+3=4 (Change)
The cut interrupts reels 1 and 4. Total: 2.

### 2

#### Input
3
1
1
1

#### Output
3

#### Explanation
There are no internal changes. Any cut drawn must interrupt all 3 scenes.

## Input Format
- The first line contains an integer $n$, the number of reels.
- The next $n$ lines each contain space-separated integers representing the durations of the scenes in that reel.

## Output Format
- Return a single integer representing the minimum number of scenes interrupted.

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

