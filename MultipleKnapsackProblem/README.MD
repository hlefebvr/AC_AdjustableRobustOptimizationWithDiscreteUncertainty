# Multiple Knapsack Problem with uncertain wights

This folder contains the instances used for the Multiple Knapsack Problem with uncertain weights application. 

## Instances

The instances can be found in the `data` folder in plain text with the following format:

```
n_knapsacks n_items
for each knapsack k: capacity(k)
for each item i: profit(i)) weight(i, 1) weight(i, 2)
```

Each instance name is formatted as `instance_mkp_N<A>_K<B>_H<C>_A<D>__<E>.txt` where each placeholder stands for the following:

- `<A>`: number of items;
- `<B>`: number of knapsacks;
- `<C>`: value of $H$ for generating the instance, multiplied by 100;
- `<D>`: value of $\alpha$ for generating the instance, multiplied by 100;
- `<E>`: instance index.
