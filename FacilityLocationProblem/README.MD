# Instances for Facilitiy Location Problem with random disruptions

## Instances

The instances are stored as plain text in the following format:
```
n_facilities n_customers
one line for each facility i: fixed_cost(i) capacity(i)
one line for each customer j: demand(j)
one line for each facility i:
  one line for each customer j:
    per_unit_transportation_cost(i, j)
```

## Results

The results come into three CSV files.

### Results obtained by CCG

These can be found in `CCG.csv` with the following columns:
- "instance": instance name 
- "gamma": value for gamma
- "iter": number of iterations
- "LB": best returned lower bound
- "UB": best returned upper bound
- "time": computation time
- "inner_iter_1": inner iteration counter (ignore)
- "inner_iter_2" inner iteration counter (ignore)

### Results obtained by B6C

These can be found in `B&C.csv` with the following columns:
- "instance": instance name
- "gamma": value for gamma
- "status": returned status
- "reason": returned reason for status (ignore)
- "objective": best returned upper bound
- "time": computation time
- "nodes": number of explored nodes
- "rel_gap": relative optimality gap
- "abs_gap": absolute optimility gap
- "n_generated_cuts": number of generated cuts

### Results obtained by B6C for increasing values of R

These can be found in `B&C_partial_disruption.csv` with the same columns as in `B&C.csv` with an extra last column for R. 

