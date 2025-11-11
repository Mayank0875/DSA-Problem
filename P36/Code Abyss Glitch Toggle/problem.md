## Title

Code Abyss: Glitch Toggle

## Slug

code-abyss-glitch-toggle

## Difficulty

Medium

## Description

A programmer is trapped in the Code Abyss and must stabilize a sequence of n code modules, numbered 1 to n. Initially, every module is in a stable (green) state.  
The programmer runs n debug passes. During the i‑th pass (for i from 1 to n), every module whose index j is a multiple of i toggles its state: a stable (green) module becomes unstable (red), and an unstable module becomes stable again.  
After completing all n passes, the programmer checks the final configuration. He needs exactly k modules to be stable (green) at the end. Determine the smallest possible number of modules n the programmer should start with to achieve exactly k stable modules.

## Examples

### 1

#### Input

1

#### Output

2

#### Explanation

If n=1, initial: [G]. Pass 1 toggles 1: [R]. Final: 0 stable.  
If n=2, initial: [G, G]. Pass 1 toggles 1, 2: [R, R]. Pass 2 toggles 2: [R, G]. Final: 1 stable (k=1).  
Smallest n is 2.

### 2

#### Input

3

#### Output

5

#### Explanation
If n=5, initial: [G,G,G,G,G].  
Pass 1 toggles 1,2,3,4,5 → [R,R,R,R,R].  
Pass 2 toggles 2,4 → [R,G,R,G,R].  
Pass 3 toggles 3 → [R,G,G,G,R].  
Pass 4 toggles 4 → [R,G,G,R,R].  
Pass 5 toggles 5 → [R,G,G,R,G].  
Final state: 3 modules (2, 3, 5) are stable (k=3). We can show n=4 results in only 2 stable modules ([R,G,G,R]), so 5 is the minimum.

## Input Format  

- The only input line has an integer k.

## Output Format  

- Return one integer: the minimum number of modules required.

## Constraints  

- 1 ≤ x ≤ 1e18

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory