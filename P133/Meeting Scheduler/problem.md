## Title
Meeting Scheduler

## Slug
meeting-scheduler

## Difficulty
Medium

## Description
A team schedule shows busy blocks for each employee. You want to schedule a brief announcement when the fewest people are busy.

There is a schedule consisting of $n$ employees. Each employee's timeline is composed of several meetings, each having a specific duration (integers). The total duration of every employee's timeline is identical.

You need to find a time slot from the start of day to the end of day of the schedule that minimizes the number of meetings it interrupts.

If the time slot passes exactly through the break between two meetings, it is **not** considered as interrupting a meeting. However, you cannot place the time slot at the very start or the very end of the schedule.

Given the 2D array `structure` containing the durations of the meetings in each employee's timeline, return the minimum number of meetings interrupted.

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
We can find a time slot at distance 4 from the start.
- Employee 1: 1+2+2=5 (Interrupt)
- Employee 2: 3+1=4 (Break)
- Employee 3: 1+3=4 (Break)
- Employee 4: 2 (Interrupt)
- Employee 5: 3+1=4 (Break)
- Employee 6: 1+3=4 (Break)
The time slot interrupts employees 1 and 4. Total: 2.

### 2

#### Input
3
1
1
1

#### Output
3

#### Explanation
There are no internal breaks. Any time slot drawn must interrupt all 3 meetings.

## Input Format
- The first line contains an integer $n$, the number of employees.
- The next $n$ lines each contain space-separated integers representing the durations of the meetings in that employee's timeline.

## Output Format
- Return a single integer representing the minimum number of meetings interrupted.

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

