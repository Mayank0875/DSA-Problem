## Title

Shadow Spectrum

## Slug

shadow-spectrum

## Difficulty

Easy

## Description

In the realm of the Shadow Spectrum, the grand sorcerer must capture exactly **n** additional shadows of a mystical artifact before the twilight ceremony begins. He possesses the original artifact and has access to two magical shadow‑capturing devices.
The first device takes **x** seconds to capture a shadow (from the original or from any already captured shadow), and the second device takes **y** seconds. The sorcerer may use either device or both simultaneously.  
Help the sorcerer determine the minimum amount of time required to produce at least **n** new shadows of the artifact, starting with just the original.

## Examples

### 1

#### Input

5 1 2

#### Output

4

#### Explanation

We need 5 shadows. Assume device 1 takes 1 s, device 2 takes 2 s.
    1. Use device 1 on the original (1 s elapsed). Now we have 2 shadows. Need 4 more.
    2. Use device 1 on original, device 2 on a shadow (2 s elapsed total, 1 s more). Device 1 finishes. Now have 3 shadows. Need 3 more.
    3. Use device 1 on original (3 s elapsed total, 1 s more). Device 2 finishes its first capture. Now have 4 shadows. Need 2 more.
    4. Use device 1 on original, device 2 on a shadow (4 s elapsed total, 1 s more). Device 1 finishes. Now have 5 shadows. Need 1 more. Device 2 finishes. Now have 6 shadows. We have enough shadows.
Minimum time is 4 seconds.

### 2

#### Input

4 1 1

#### Output

3

#### Explanation

Need 4 shadows. Both devices take 1 s.
    1. Use device 1 on original (1 s). Have 2 shadows. Need 3 more.
    2. Use device 1 and 2 on the available shadows (2 s). Have 4 shadows. Need 1 more.
    3. Use device 1 and 2 again (3 s). Have 6 shadows. We have enough.
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