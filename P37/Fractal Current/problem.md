## Title

Fractal Current

## Slug

fractal-current

## Difficulty

Easy

## Description

A researcher is studying a fractal phenomenon and needs to generate exactly **n** additional fractal instances before the observation window closes. The lab has two fractal generators.
The first generator creates a new fractal instance from any existing one in **x** seconds, and the second generator does the same in **y** seconds. The researcher can operate either generator or both simultaneously.  
Determine the minimum amount of time required to produce at least **n** new fractal instances, starting with just the original fractal.

## Examples

### 1

#### Input

5 1 2

#### Output

4

#### Explanation

We need 5 copies. Assume generator 1 takes 1 s, generator 2 takes 2 s.
    1. Use generator 1 on the original (1 s elapsed). Now we have 2 fractals. Need 4 more.
    2. Use generator 1 on original, generator 2 on a copy (2 s elapsed total, 1 s more). Generator 1 finishes. Now have 3 fractals. Need 3 more.
    3. Use generator 1 on original (3 s elapsed total, 1 s more). Generator 2 finishes its first copy. Now have 4 fractals. Need 2 more.
    4. Use generator 1 on original, generator 2 on a copy (4 s elapsed total, 1 s more). Generator 1 finishes. Now have 5 fractals. Need 1 more. Generator 2 finishes. Now have 6 fractals. We have enough copies.
Minimum time is 4 seconds.

### 2

#### Input

4 1 1

#### Output

3

#### Explanation

Need 4 copies. Both generators take 1 s.
    1. Use generator 1 on original (1 s). Have 2 fractals. Need 3 more.
    2. Use generator 1 and 2 on the available fractals (2 s). Have 4 fractals. Need 1 more.
    3. Use generator 1 and 2 again (3 s). Have 6 fractals. We have enough.
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