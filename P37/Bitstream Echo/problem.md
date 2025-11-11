## Title

Bitstream Echo

## Slug

bitstream-echo

## Difficulty

Easy

## Description

An audio engineer needs to generate at least **n** additional copies of a digital bitstream before a live broadcast starts. The original bitstream is available, and there are two echo processors that can duplicate it.
The first processor takes **x** seconds to copy one bitstream (from the original or any existing copy), and the second processor takes **y** seconds. The engineer can use either processor or both simultaneously.  
Help determine the minimum amount of time required to produce at least **n** new copies of the bitstream, starting with just the original.

## Examples

### 1

#### Input

5 1 2

#### Output

4

#### Explanation

We need 5 copies. Assume processor 1 takes 1 s, processor 2 takes 2 s.
    1. Use processor 1 on the original (1 s elapsed). Now we have 2 bitstreams. Need 4 more.
    2. Use processor 1 on original, processor 2 on a copy (2 s elapsed total, 1 s more). Processor 1 finishes. Now have 3 bitstreams. Need 3 more.
    3. Use processor 1 on original (3 s elapsed total, 1 s more). Processor 2 finishes its first copy. Now have 4 bitstreams. Need 2 more.
    4. Use processor 1 on original, processor 2 on a copy (4 s elapsed total, 1 s more). Processor 1 finishes. Now have 5 bitstreams. Need 1 more. Processor 2 finishes. Now have 6 bitstreams. We have enough copies.
Minimum time is 4 seconds.

### 2

#### Input

4 1 1

#### Output

3

#### Explanation

Need 4 copies. Both processors take 1 s.
    1. Use processor 1 on original (1 s). Have 2 bitstreams. Need 3 more.
    2. Use processor 1 and 2 on the available bitstreams (2 s). Have 4 bitstreams. Need 1 more.
    3. Use processor 1 and 2 again (3 s). Have 6 bitstreams. We have enough.
Minimum time is 3 seconds.
  
## Input Format  

- Three space-separated integers n, x, and y.

## Output Format  

- Return single integer representing the minimum time in seconds required.
  

## Constraints  

- 1 ≤ n ≤ 1e8
- 1 ≤ x, y ≤ 10

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory