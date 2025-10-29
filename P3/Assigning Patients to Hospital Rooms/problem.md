## Title

Assigning Patients to Hospital Rooms

## Slug

assigning-patients-hospital-rooms

## Difficulty

Easy

## Description

A hospital needs to assign patients to recovery rooms. Each room can accommodate one or two patients. For safety or resource reasons, the combined 'severity index' (a numerical value) of patients in a single room cannot exceed a limit `x`. You are given the severity indices for `n` patients. Find the minimum number of rooms required to place all patients, adhering to the severity limit per room.

## Examples

### 1

#### Input

4 10
[7, 2, 3, 9]

#### Output

3

#### Explanation

One minimal room assignment:
    - Room 1: Patient with index 2 and patient with index 7 (Total index 9 <= 10)
    - Room 2: Patient with index 3 (Total index 3 <= 10)
    - Room 3: Patient with index 9 (Total index 9 <= 10)
This requires 3 rooms.

### 2

#### Input

5 5
[2, 2, 2, 3, 4]

#### Output

3

#### Explanation

One minimal room assignment:
    - Room 1: Patient with index 2 and patient with index 3 (Total index 5 <= 5)
    - Room 2: Two patients with index 2 (Total index 4 <= 5)
    - Room 3: Patient with index 4 (Total index 4 <= 5)
This requires 3 rooms.

## Input Format

- The first line contains two integers n and x: the number of patients and the maximum combined severity index per room.
- The second line contains n integers p_1, p_2, ..., p_n: the severity index of each patient.

## Output Format

- Return a single integer: the minimum number of rooms required.

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