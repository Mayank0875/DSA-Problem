## Title
Server Request Batching

## Slug
server-request-batching

## Difficulty
Hard

## Description
A load balancer distributes a stream of `n` incoming requests to `k` servers. The requests have different processing costs and must be assigned in contiguous batches. The 'load stress' on a server is the square of the total processing cost of its batch.

You must partition the sequence of requests into exactly `k` non-empty contiguous batches.
Each batch corresponds to a server.
The "load stress" for a server is calculated as the **square of the sum** of the costs of the requests in that batch.

Your goal is to minimize the total load stress (the sum of the load stress values of all `k` batches).

## Examples

### 1

#### Input
8 3
2 3 1 2 2 3 4 1

#### Output
110

#### Explanation
We partition the requests into 3 batches: `[2, 3, 1]`, `[2, 2, 3]`, and `[4, 1]`.
The sums are 6, 7, 5.
The total load stress is $6^2 + 7^2 + 5^2 = 36 + 49 + 25 = 110$.

### 2

#### Input
5 1
1 2 3 4 5

#### Output
225

#### Explanation
Only 1 batch is allowed, containing all requests. Sum = 15. load stress = $15^2 = 225$.

## Input Format
- The first line contains two integers `n` and `k`: the number of requests and the required number of batches.
- The second line contains `n` integers representing the costs of each request.

## Output Format
- Return one integer: the minimum total load stress.

## Constraints
- 1 ≤ k ≤ n ≤ 3000
- 1 ≤ value ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, array
