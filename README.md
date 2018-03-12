# knapsack-algorithms

This is a simple Python script that demonstrates the following algorithms:

* Optimal greedy solution for [fractional (continuous) knapsack problem](https://en.wikipedia.org/wiki/Continuous_knapsack_problem)

* Recursive top-down solution for the [discrete 0-1 knapsack problem](https://en.wikipedia.org/wiki/Knapsack_problem#Definition)

* [Dynamic programming solution](https://en.wikipedia.org/wiki/Knapsack_problem#0/1_knapsack_problem) for the discrete 0-1 knapsack problem

* Recursive top-down solution with memoization for the discrete 0-1 knapsack problem

The script also counts the number of recursive calls for the recursive
solutions to 0-1 knapsack and the number of iterations for the dynamic
programming solution.

In the 0-1 knapsack problem, you're given a set of items, each of
which has a value and a weight, and a knapsack with a maximum weight
capacity. The object is to select a subset of the items to put into
the knapsack such that the sum of the values of items in the knapsack
is maximized (you can't pick another subset more valuable) but the sum
of the weights of items in the knapsack does not exceed the maximum
weight capacity. For each item, you can either select it once, or not
select it at all; so, you can't select an item more than once, or
select a fraction of an item, for example.

In the fractional knapsack problem, the object is the same, but you're
allowed to select fractions of each item. For example, if an item has
value 20 and weight 40, you can select 0.5 (half) of the item,
yielding a value of 10 and a weight of 20. You can only select at most
one of each item.

## Example Usage

To run the script simply execute it on the command line.

```
./knapsack.py
```

It will produce an output that should look like the file
[knapsack-output.txt](knapsack-output.txt).

To modify the set of items from which you can select to put into the
knapsack, modify the top of the script [knapsack.py](knapsack.py).

```
items = [ [20, 50], [15, 45], [10, 35], [20, 35], [25, 30], [30, 30], [15, 20], [10, 15], [5, 10], [20, 10] ]
weight_capacity = 166
```

Each pair represents an item, the first value is the item's value and
the second is its weight. The variable weight_capacity is the total
weight that can fit into the knapsack. 

## License

This project is licensed under the MIT License (see the [LICENSE](LICENSE) file for details).

## Authors

* **Michael Gabilondo** - [mgabilo](https://github.com/mgabilo)
