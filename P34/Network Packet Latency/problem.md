## Title

Network Packet Latency

## Slug

network-packet-latency

## Difficulty

Medium

## Description

In a simulation of a network with $n$ nodes, $n$ different types of data packets are being tested. The nodes and packet types are both ranked by priority from 1 to $n$. The latency (delay) for node $i$ to process packet type $j$ is $i \times j$ milliseconds.You need to find the median latency from all $n^2$ node-packet pairs to evaluate the network's average performance. You are given that $n$ is odd.

## Examples

### 1

#### Input

3

#### Output

3

#### Explanation

The numbers in increasing order are [1,2,2,3,3,4,6,6,9], so the answer is 3. 
    
### 2

#### Input

5

#### Output

8

#### Explanation
The middle element is 8.
  

## Input Format  

- The only input line has an integer n.

## Output Format  

- Return one integer: the answer to the task.
  

## Constraints  

- 1 ≤ x ≤ 1e6

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory