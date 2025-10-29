## Title

Log Event Window XOR Hash

## Slug

log-event-window-xor-hash

## Difficulty

Easy

## Description

A system administrator analyzes a sequence of numerical event IDs A₁, A₂, ..., Aₙ from server logs. To identify patterns in event sequences over short durations, they use a sliding window of size K. For each window, a hash is calculated by XORing the event IDs within it. To get a single hash representing the overall event pattern structure, all window hashes are XORed together. Calculate this final event pattern hash.

## Examples

### 1

#### Input

5 3
[1, 2, 3, 4, 5]

#### Output

7

#### Explanation

Event ID windows of size 3:
    •   [1, 2, 3] → Window Hash (XOR) = 0
    •   [2, 3, 4] → Window Hash (XOR) = 5
    •   [3, 4, 5] → Window Hash (XOR) = 2

Final Pattern Hash = 0 ^ 5 ^ 2 = 7

### 2

#### Input

4 2
[5, 1, 3, 2]

#### Output

7

#### Explanation

Windows:
    •   [5, 1] → XOR = 4
    •   [1, 3] → XOR = 2
    •   [3, 2] → XOR = 1

Final Pattern Hash = 4 ^ 2 ^ 1 = 7

## Input Format

- The first line contains two integers N (number of events) and K (window size).
- The second line contains N space-separated integers — the event IDs.

## Output Format

- Return a single integer — the final event pattern hash.

## Constraints

- 1 ≤ N ≤ 10^5
- 1 ≤ K ≤ N
- 0 ≤ arr[i] ≤ 1e9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

arrays, sliding window, logs, bit manipulation