## Title
Neural Network Synapses

## Slug
neural-network-synapses

## Difficulty
Medium

## Description
Two layers of artificial neurons need robust synaptic connections to prevent signal loss.

Two parallel layers, Input Layer and Hidden Layer, each contain n neurons arranged in a line.
Input Layer has an array `a` representing the activation potential of each neuron.
Hidden Layer has an array `b` representing the activation potential of each neuron.

Inside each layer, adjacent neurons are already connected by internal lateral inhibitions.

You must establish inter-layer synapses connecting some neurons of Input Layer to some neurons of Hidden Layer.

The cost to create a synapse between neuron i of Input Layer and neuron j of Hidden Layer is:
absolute value of (a[i] - b[j]).

**Fault-tolerance requirement:**
The final network must remain fully connected even if any single neuron is removed (from either Input Layer or Hidden Layer).
If one neuron fails and disappears along with all its connections, the remaining neurons must still form a single connected network.

Your task is to calculate the minimum total cost required to build such a set of connections.

## Examples

### 1

#### Input
3
1 10 1
20 4 25

#### Output
31

#### Explanation
It's optimal to connect four pairs of neurons:
1. neuron 1 from Input Layer with neuron 2 from Hidden Layer: cost |1-4| = 3.
2. neuron 3 from Input Layer with neuron 2 from Hidden Layer: cost |1-4| = 3.
3. neuron 2 from Input Layer with neuron 1 from Hidden Layer: cost |10-20| = 10.
4. neuron 2 from Input Layer with neuron 3 from Hidden Layer: cost |10-25| = 15.
Total cost: 3 + 3 + 10 + 15 = 31.

### 2

#### Input
4
1 1 1 1
1000000000 1000000000 1000000000 1000000000

#### Output
1999999998

#### Explanation
It is optimal to connect the first neuron of Input Layer with the first of Hidden Layer, and the last neuron of Input Layer with the last of Hidden Layer, satisfying the connectivity conditions efficiently given the values.

## Input Format
- The first line contains an integer n, the number of neurons in each layer.
- The second line contains n integers representing the activation potentials of Input Layer.
- The third line contains n integers representing the activation potentials of Hidden Layer.

## Output Format
- Return a single integer representing the minimum total cost to make the network fault-tolerant.

## Constraints
- 3 ≤ n ≤ 10^5
- 1 ≤ a[i], b[i] ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, greedy, math
