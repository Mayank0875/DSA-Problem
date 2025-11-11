## Title

Static Field Activation

## Slug

static-field

## Difficulty

Medium

## Description

A researcher sets up a static field with n sensors arranged in a line, numbered 1 to n. Initially, all sensors are active.  
The researcher then performs n field pulses. For the i‑th pulse (where i goes from 1 to n), every sensor whose number j is a multiple of i toggles its state: an active sensor becomes inactive, and an inactive sensor becomes active. After all n pulses have been applied, the researcher observes the final configuration of the sensors. The researcher needs exactly k sensors to remain active in the end. Find the smallest possible number of sensors n the researcher should start with to achieve exactly k active sensors.

## Examples

### 1

#### Input

1

#### Output

2

#### Explanation

If n=1, initial: [A]. Pulse 1 toggles 1: [I]. Final: 0 active.  
If n=2, initial: [A, A]. Pulse 1 toggles 1, 2: [I, I]. Pulse 2 toggles 2: [I, A]. Final: 1 active (k=1).  
Smallest n is 2.
    
### 2

#### Input

3

#### Output

5

#### Explanation
If n=5, initial: [A,A,A,A,A].  
Pulse 1 toggles 1,2,3,4,5 → [I,I,I,I,I].  
Pulse 2 toggles 2,4 → [I,A,I,A,I].  
Pulse 3 toggles 3 → [I,A,A,A,I].  
Pulse 4 toggles 4 → [I,A,A,I,I].  
Pulse 5 toggles 5 → [I,A,A,I,A].  
Final state: 3 sensors (2, 3, 5) are active (k=3). We can show n=4 results in only 2 active sensors ([I,A,A,I]), so 5 is the minimum.
  

## Input Format  

- The only input line has an integer k.

## Output Format  

- Return one integer: the minimum number of sensors required.
  

## Constraints  

- 1 ≤ x ≤ 1e18

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory