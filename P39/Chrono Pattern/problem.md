## Title

Chrono Pattern

## Slug

chrono-pattern

## Difficulty

Easy

## Description

Imagine a timeline of events, each with a distinct magnitude. As you examine each event, you look back in time (to earlier events) and want to know the magnitude of the nearest earlier event that is strictly greater than the current one. If all previous events are smaller or equal in magnitude, or if it is the first event, there is no such greater event in the past. Your goal is to determine this greater event's magnitude for each position along the timeline.

## Examples

### 1

#### Input

8
[30, 60, 90, 50, 80, 40, 70, 50]

#### Output

[-1, -1, -1, 90, 90, 80, 80, 70]

#### Explanation

Event 0 (30): No previous event. Output -1.
Event 1 (60): Event 0 (30) is smaller. Output -1.
Event 2 (90): Events 0 (30), 1 (60) are smaller. Output -1.
Event 3 (50): Event 2 (90) is the nearest greater. Output 90.
Event 4 (80): Event 2 (90) is the nearest greater. Output 90.
Event 5 (40): Event 4 (80) is the nearest greater. Output 80.
Event 6 (70): Event 4 (80) is the nearest greater. Output 80.
Event 7 (50): Event 6 (70) is the nearest greater. Output 70.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All events have equal magnitude, so no strictly greater previous event exists.

## Input Format

The first line contains a single integer n, the number of events.
The second line contains n space-separated integers h_0, h_1, ..., h_[n-1], representing the magnitude of each event.

## Output Format

Return array of integers. The i-th integer should be the magnitude of the nearest event j < i such that h_j > h_i. If no such day exists, then -1.

## Constraints

1 ≤ n ≤ 10^5
1 ≤ h_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array