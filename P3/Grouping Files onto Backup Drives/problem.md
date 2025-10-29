## Title

Grouping Files onto Backup Drives

## Slug

grouping-files-backup-drives

## Difficulty

Easy

## Description

You need to back up a collection of digital files onto backup drives. Each drive can store either one or two files. Due to storage limitations, the total size of the files on a single drive cannot exceed `x` gigabytes. You are given the sizes of `n` files. Calculate the minimum number of backup drives needed to store all the files without exceeding the size limit on any drive.

## Examples

### 1

#### Input

4 10
[7, 2, 3, 9]

#### Output

3

#### Explanation

One efficient grouping is:
    - Drive 1: File of size 2GB and file of size 7GB (Total size 9 <= 10)
    - Drive 2: File of size 3GB (Total size 3 <= 10)
    - Drive 3: File of size 9GB (Total size 9 <= 10)
This requires 3 drives.

### 2

#### Input

5 5
[2, 2, 2, 3, 4]

#### Output

3

#### Explanation

One efficient grouping is:
    - Drive 1: File of size 2GB and file of size 3GB (Total size 5 <= 5)
    - Drive 2: Two files of size 2GB (Total size 4 <= 5)
    - Drive 3: File of size 4GB (Total size 4 <= 5)
This requires 3 drives.

## Input Format

- The first line contains two integers n and x: the number of files and the maximum allowed size per drive (in GB).
- The second line contains n integers p_1, p_2, ..., p_n: the size of each file (in GB).

## Output Format

- Return a single integer: the minimum number of backup drives required.

## Constraints

- 1 ≤ n ≤ 1e5
- 1 ≤ x ≤ 1e9
- 1 ≤ p_i ≤ x

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

greedy, sorting, two pointers