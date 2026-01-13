## Title
Log Cabin Wall

## Slug
log-cabin-wall

## Difficulty
Medium

## Description
A cabin wall is made of logs. You want to cut a window opening that saws through the fewest logs (hitting chinking/gaps).

There is a wall consisting of $n$ courses. Each course is composed of several logs, each having a specific length (integers). The total length of every course is identical.

You need to cut a window side from the top to the bottom of the wall that minimizes the number of logs it saws.

If the window side passes exactly through the chinking between two logs, it is **not** considered as sawing a log. However, you cannot place the window side at the very left or the very right of the wall.

Given the 2D array `structure` containing the lengths of the logs in each course, return the minimum number of logs sawed.

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
We can cut a window side at distance 4 from the left.
- Course 1: 1+2+2=5 (Saw)
- Course 2: 3+1=4 (Chinking)
- Course 3: 1+3=4 (Chinking)
- Course 4: 2 (Saw)
- Course 5: 3+1=4 (Chinking)
- Course 6: 1+3=4 (Chinking)
The window side saws courses 1 and 4. Total: 2.

### 2

#### Input
3
1
1
1

#### Output
3

#### Explanation
There are no internal chinkings. Any window side drawn must saw all 3 logs.

## Input Format
- The first line contains an integer $n$, the number of courses.
- The next $n$ lines each contain space-separated integers representing the lengths of the logs in that course.

## Output Format
- Return a single integer representing the minimum number of logs sawed.

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

