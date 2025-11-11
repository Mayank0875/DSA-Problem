## Title

Static Field Deployment

## Slug

static-field-deployment

## Difficulty

Easy

## Description

The research lab needs to generate a static electromagnetic field at multiple locations for an upcoming experiment. The lead scientist has one prototype field generator and must create exactly **n** additional field generators before the experiment begins. There are two fabrication units available.

The first fabrication unit takes **x** seconds to produce one field generator (from the original prototype or any already produced generator), and the second unit takes **y** seconds. The scientists can operate either unit or both simultaneously.

Help the lead scientist determine the minimum amount of time required to produce at least **n** new field generators, starting with just the original prototype.

## Examples

### 1

#### Input

5 1 2

#### Output

4

#### Explanation

We need 5 copies. Assume unit 1 takes 1 s, unit 2 takes 2 s.
    1. Use unit 1 on the original (1 s elapsed). Now we have 2 generators. Need 4 more.
    2. Use unit 1 on original, unit 2 on a copy (2 s elapsed total, 1 s more). Unit 1 finishes. Now have 3 generators. Need 3 more.
    3. Use unit 1 on original (3 s elapsed total, 1 s more). Unit 2 finishes its first copy. Now have 4 generators. Need 2 more.
    4. Use unit 1 on original, unit 2 on a copy (4 s elapsed total, 1 s more). Unit 1 finishes. Now have 5 generators. Need 1 more. Unit 2 finishes. Now have 6 generators. We have enough copies.
Minimum time is 4 seconds.

### 2

#### Input

4 1 1

#### Output

3

#### Explanation

Need 4 copies. Both units take 1 s.
    1. Use unit 1 on original (1 s). Have 2 generators. Need 3 more.
    2. Use unit 1 and 2 on the available generators (2 s). Have 4 generators. Need 1 more.
    3. Use unit 1 and 2 again (3 s). Have 6 generators. We have enough.
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