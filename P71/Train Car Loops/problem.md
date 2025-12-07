## Title
Train Car Loops

## Slug
train-car-loops

## Difficulty
Medium

## Description
Toy train cars are hooked together to form closed loops. Each car connects to one in front and one behind.

There are n train cars.
Loops consist of at least 2 cars.
We can only see the coupling on one end of each car.

Your task is to analyze this partial data and determine the minimum and maximum number of separate loops that could possibly exist, consistent with the given records.

## Examples

### 1

#### Input
6
2 1 4 3 6 5

#### Output
1 3

#### Explanation
The records show the connections:
1 <-> 2,
3 <-> 4,
5 <-> 6.
Maximum:
These could be 3 separate loops of 2 cars each.
Minimum:
Since we only know one neighbor per car, these pairs could actually be segments of a bigger ring. All cars can be arranged into one single ring:
1 - 2 - 3 - 4 - 5 - 6 - 1.

### 2

#### Input
6
2 3 1 5 6 4

#### Output
2 2

#### Explanation
Maximum: 2
Minimum: 2
(Two cycles of length 3 are formed, which are fixed).

## Input Format
- The first line contains an integer n, the number of cars.
- The second line contains n space-separated integers a1, a2, ..., an, where ai is the neighbor remembered by the i-th car.

## Output Format
- Return two integers: the minimum number of loops and the maximum number of loops.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ ai ≤ 2e5
- ai ≠ i
- The input guarantees that a valid configuration of loops exists.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, depth-first-search, connected-components
