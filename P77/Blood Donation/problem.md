## Title
Blood Donation

## Slug
blood-donation

## Difficulty
Medium

## Description
There are `n` donors and `m` patients in need of blood transfusions.

However, not every donor is compatible with every patient based on blood type compatibility.
You are given a list of `k` compatible pairs, where a specific donor can work with a specific patient.

Your task is to determine the maximum number of transfusions that can be formed simultaneously. Each donor and each patient can be assigned to at most one transfusion.

## Examples

### 1

#### Input
3 2 4
1 1
1 2
2 1
3 1

#### Output
2

#### Explanation
There are 3 donors and 2 patients.
Possible valid matching could be:
- donor 1 with patient 2
- donor 2 with patient 1
Total = 2.

### 2

#### Input
2 2 1
1 1

#### Output
1

#### Explanation
Only donor 1 and patient 1 are compatible. The maximum number of operational transfusions is 1.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of donors, patients, and compatible pairs.
- The donors are numbered `1` to `n` and the patients are numbered `1` to `m`.
- The next `k` lines describe the compatible pairs. Each line contains two integers `a` and `b`, indicating that donor `a` and patient `b` are compatible.

## Output Format
- Return one integer: the maximum number of pairs that can be formed.

## Constraints
- 1 ≤ n, m ≤ 500
- 1 ≤ k ≤ 1000
- 1 ≤ a ≤ n
- 1 ≤ b ≤ m

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph
