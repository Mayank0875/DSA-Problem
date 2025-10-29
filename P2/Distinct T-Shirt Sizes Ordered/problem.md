## Title

Distinct T-Shirt Sizes Ordered

## Slug

distinct-tshirt-sizes-ordered

## Difficulty

Easy

## Description

A clothing store is analyzing T-shirt sales data. Each size (like S, M, L, XL) is represented by a numerical code. The sales log contains the size code for every T-shirt sold. To manage inventory effectively, the store manager needs to know how many different T-shirt sizes were sold in total. Given the list of size codes from the sales log, calculate the number of unique sizes that had at least one sale.

## Examples

### 1

#### Input

5
[2, 3, 2, 2, 3]

#### Output

2

#### Explanation

The size codes sold are 2, 3, 2, 2, 3. The unique size codes are 2 and 3. The store sold 2 distinct T-shirt sizes.

### 2

#### Input

8
[10, 5, 10, 2, 5, 10, 5, 2]

#### Output

3

#### Explanation

The unique size codes are 10, 5, and 2. The store sold 3 distinct T-shirt sizes.

## Input Format

- The first line contains an integer n: the total number of T-shirts sold.
- The second line contains $n$ integers x_1, x_2, ...., x_n: the T-shirt size codes.

## Output Format

- Return a single integer: the count of distinct size codes.

## Constraints

- 1 ≤ n ≤ 1e5
- 1 ≤ x_i ≤ 1e9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

sorting, set, counting, retail