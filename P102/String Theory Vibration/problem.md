## Title
String Theory Vibration

## Slug
string-theory-vibration

## Difficulty
Hard

## Description
In a simulation, a 1D string with $n$ harmonic nodes is split. The energy cost depends on the vibrational modes.

The separation process involves splitting the string or any of its resulting fragments into two parts. You can choose any fragment consisting of more than one node and split it at any valid boundary between nodes. However, the process consumes resources. The cost of a single split is equal to the sum of the energy of all nodes in the fragment being split.

Your task is to determine the minimum total cost required to break the entire string down into single isolated nodes.

## Examples

### 1

#### Input
5 
2 7 3 2 5

#### Output
43

#### Explanation
One optimal strategy involves splitting the sequence `[2, 7, 3, 2, 5]` (sum 19) into `[2, 7]` (sum 9) and `[3, 2, 5]` (sum 10). Cost so far: 19.
Then split `[2, 7]` into `[2]` and `[7]`. Cost: 19 + 9 = 28.
Then split `[3, 2, 5]` into `[3, 2]` (sum 5) and `[5]`. Cost: 28 + 10 = 38.
Finally split `[3, 2]` into `[3]` and `[2]`. Cost: 38 + 5 = 43.

### 2

#### Input
1
1

#### Output
0

#### Explanation
Already a single element, so the cost is 0.

## Input Format
- The first line contains an integer $n$: the number of nodes.
- The second line contains $n$ integers representing the energy of each node.

## Output Format
- Return one integer: the minimum total cost to separate all nodes.

## Constraints
- 1 ≤ n ≤ 5000
- 1 ≤ value ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, divide-and-conquer, knuth-optimization
