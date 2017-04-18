## 1. Breadth first search
### Air Cargo Problem 1
 - Expansions: 43
 - Goal Tests: 56
 - New Nodes: 180
 - Plan length: 6
 - Execution time: 0.03547631500987336 seconds
```
Load(C1, P1, SFO)
Load(C2, P2, JFK)
Fly(P2, JFK, SFO)
Unload(C2, P2, SFO)
Fly(P1, SFO, JFK)
Unload(C1, P1, JFK)
```

### Air Cargo Problem 2
 - Expansions: 3346
 - Goal Tests: 4612
 - New Nodes: 30534
 - Plan length: 9
 - Execution time: 81.65928123100002 seconds
```
Load(C1, P1, SFO)
Load(C2, P2, JFK)
Load(C3, P3, ATL)
Fly(P1, SFO, JFK)
Unload(C1, P1, JFK)
Fly(P2, JFK, SFO)
Unload(C2, P2, SFO)
Fly(P3, ATL, SFO)
Unload(C3, P3, SFO)
```

### Air Cargo Problem 3
 - Expansions: 14663
 - Goal Tests: 18098
 - New Nodes: 129631
 - Plan length: 12
 - Execution time: 457.6173511959996 seconds
```
Load(C1, P1, SFO)
Load(C2, P2, JFK)
Fly(P2, JFK, ORD)
Load(C4, P2, ORD)
Fly(P1, SFO, ATL)
Load(C3, P1, ATL)
Fly(P1, ATL, JFK)
Unload(C1, P1, JFK)
Unload(C3, P1, JFK)
Fly(P2, ORD, SFO)
Unload(C2, P2, SFO)
Unload(C4, P2, SFO)
```

## 2. Breadth first tree search
### Air Cargo Problem 1
 - Expansions: 1458
 - Goal Tests: 1459
 - New Nodes: 5960
 - Plan length: 6
 - Execution time: 6.019270433000202 seconds
```
Load(C1, P1, SFO)
Load(C2, P2, JFK)
Fly(P2, JFK, SFO)
Unload(C2, P2, SFO)
Fly(P1, SFO, JFK)
Unload(C1, P1, JFK)
```
### Air Cargo Problem 2
Does not terminate in 10 minutes.

### Air Cargo Problem 3
Does not terminate in 10 minutes.


## 3. Depth first graph search
### Air Cargo Problem 1
 - Expansions: 21
 - Goal Tests: 22
 - New Nodes: 84
 - Plan length: 20
 - Execution time: 0.09816352300003928 seconds
```
Fly(P1, SFO, JFK)
Fly(P2, JFK, SFO)
Load(C2, P1, JFK)
Fly(P1, JFK, SFO)
Fly(P2, SFO, JFK)
Unload(C2, P1, SFO)
Fly(P1, SFO, JFK)
Fly(P2, JFK, SFO)
Load(C2, P2, SFO)
Fly(P1, JFK, SFO)
Load(C1, P2, SFO)
Fly(P2, SFO, JFK)
Fly(P1, SFO, JFK)
Unload(C2, P2, JFK)
Unload(C1, P2, JFK)
Fly(P2, JFK, SFO)
Load(C2, P1, JFK)
Fly(P1, JFK, SFO)
Fly(P2, SFO, JFK)
Unload(C2, P1, SFO)
```

### Air Cargo Problem 2
 - Expansions: 107
 - Goal Tests: 108
 - New Nodes: 959
 - Plan length: 105
 - Execution time: 2.255084823999823 seconds
```
Fly(P3, ATL, JFK)
Fly(P2, JFK, ATL)
Fly(P3, JFK, SFO)
Fly(P2, ATL, SFO)
Fly(P1, SFO, ATL)
Fly(P3, SFO, ATL)
Fly(P1, ATL, JFK)
Fly(P3, ATL, JFK)
...
Unload(C2, P3, SFO)
```

### Air Cargo Problem 3
 - Expansions: 408
 - Goal Tests: 409
 - New Nodes: 3364
 - Plan length: 392
 - Execution time: 11.076630202999695 seconds
```
Fly(P1, SFO, ORD)
Fly(P2, JFK, ORD)
Fly(P1, ORD, ATL)
Fly(P2, ORD, ATL)
Fly(P1, ATL, JFK)
Fly(P2, ATL, SFO)
...
Unload(C3, P1, JFK)
```

## 4. Depth limited search
### Air Cargo Problem 1
 - Expansions: 101
 - Goal Tests: 271
 - New Nodes: 414
 - Plan length: 50
 - Execution time: 0.48083225499794935 seconds
```
Load(C1, P1, SFO)
Load(C2, P2, JFK)
Unload(C1, P1, SFO)
Load(C1, P1, SFO)
Unload(C1, P1, SFO)
Load(C1, P1, SFO)
Unload(C1, P1, SFO)
...
Unload(C1, P1, JFK)
```

### Air Cargo Problem 2
Does not terminate in 10 minutes.

### Air Cargo Problem 3
Does not terminate in 10 minutes.

## 5. Uniform cost search
### Air Cargo Problem 1
 - Expansions: 55
 - Goal Tests: 57
 - New Nodes: 224
 - Plan length: 6
 - Execution time: 0.2418411139951786 seconds
```
Load(C1, P1, SFO)
Load(C2, P2, JFK)
Fly(P1, SFO, JFK)
Fly(P2, JFK, SFO)
Unload(C1, P1, JFK)
Unload(C2, P2, SFO)
 ```

### Air Cargo Problem 2
 - Expansions: 4853
 - Goal Tests: 4855
 - New Nodes: 44041
 - Plan length: 9
 - Execution time: 140.8912663539959 seconds
```
Load(C1, P1, SFO)
Load(C2, P2, JFK)
Load(C3, P3, ATL)
Fly(P1, SFO, JFK)
Fly(P2, JFK, SFO)
Fly(P3, ATL, SFO)
Unload(C3, P3, SFO)
Unload(C2, P2, SFO)
Unload(C1, P1, JFK)
```

### Air Cargo Problem 3
Does not terminate in 10 minutes.

## 6. Recursive best first search with h1 heuristic function
### Air Cargo Problem 1
 - Expansions: 4229
 - Goal Tests: 4230
 - New Nodes: 17023
 - Plan length: 6
 - Execution time: 17.971775871999853 seconds
```
Load(C2, P2, JFK)
Load(C1, P1, SFO)
Fly(P2, JFK, SFO)
Unload(C2, P2, SFO)
Fly(P1, SFO, JFK)
Unload(C1, P1, JFK)
```

### Air Cargo Problem 2
Does not terminate in 10 minutes.

### Air Cargo Problem 3
Does not terminate in 10 minutes.

## 7. Greedy best first graph search with h_1
### Air Cargo Problem 1
 - Expansions: 7
 - Goal Tests: 9
 - New Nodes: 28
 - Plan length: 6
 - Execution time: 0.02786448599999858 seconds
```
Load(C1, P1, SFO)
Load(C2, P2, JFK)
Fly(P1, SFO, JFK)
Fly(P2, JFK, SFO)
Unload(C1, P1, JFK)
Unload(C2, P2, SFO)
```

### Air Cargo Problem 2
 - Expansions: 998
 - Goal Tests: 1000
 - New Nodes: 8982
 - Plan length: 21
 - Execution time: 26.12001982899983 seconds
```
Load(C1, P1, SFO)
Load(C2, P2, JFK)
Load(C3, P3, ATL)
Fly(P1, SFO, ATL)
Fly(P2, JFK, ATL)
Fly(P3, ATL, JFK)
Fly(P2, ATL, SFO)
Unload(C2, P2, SFO)
Fly(P2, SFO, ATL)
Fly(P3, JFK, SFO)
Load(C2, P3, SFO)
Fly(P3, SFO, JFK)
Fly(P1, ATL, JFK)
Unload(C1, P1, JFK)
Load(C1, P3, JFK)
Fly(P1, JFK, ATL)
Fly(P3, JFK, SFO)
Unload(C3, P3, SFO)
Unload(C2, P3, SFO)
Fly(P3, SFO, JFK)
Unload(C1, P3, JFK)
```

### Air Cargo Problem 3
 - Expansions: 5614
 - Goal Tests: 5616
 - New Nodes: 49429
 - Plan length: 22
 - Execution time: 259.74592149100044 seconds
```
Load(C1, P1, SFO)
Load(C2, P2, JFK)
Fly(P1, SFO, ORD)
Load(C4, P1, ORD)
Fly(P2, JFK, ATL)
Load(C3, P2, ATL)
Fly(P2, ATL, ORD)
Fly(P1, ORD, ATL)
Unload(C4, P1, ATL)
Fly(P1, ATL, ORD)
Fly(P2, ORD, ATL)
Load(C4, P2, ATL)
Fly(P2, ATL, ORD)
Unload(C3, P2, ORD)
Load(C3, P1, ORD)
Fly(P1, ORD, JFK)
Unload(C3, P1, JFK)
Unload(C1, P1, JFK)
Fly(P1, JFK, ORD)
Fly(P2, ORD, SFO)
Unload(C4, P2, SFO)
Unload(C2, P2, SFO)
```

## 8. A* search with h1 heuristic function
### Air Cargo Problem 1

### Air Cargo Problem 2

### Air Cargo Problem 3

## 9. A* search with h_ignore_preconditions
### Air Cargo Problem 1
 - Expansions: 41
 - Goal Tests: 43
 - New Nodes: 170
 - Plan length: 6
 - Execution time: 0.042065354995429516 seconds
```
Load(C1, P1, SFO)
Fly(P1, SFO, JFK)
Unload(C1, P1, JFK)
Load(C2, P2, JFK)
Fly(P2, JFK, SFO)
```

### Air Cargo Problem 2
 - Expansions: 1506
 - Goal Tests: 1508
 - New Nodes: 13820
 - Plan length: 9
 - Execution time: 13.943244863010477 seconds
```
Load(C3, P3, ATL)
Fly(P3, ATL, SFO)
Unload(C3, P3, SFO)
Load(C2, P2, JFK)
Fly(P2, JFK, SFO)
Unload(C2, P2, SFO)
Load(C1, P1, SFO)
Fly(P1, SFO, JFK)
Unload(C1, P1, JFK)
```

### Air Cargo Problem 3
 - Expansions: 5118
 - Goal Tests: 5120
 - New Nodes: 45650
 - Plan length: 12
 - Execution time: 93.62522890602122 seconds
```
Load(C2, P2, JFK)
Fly(P2, JFK, ORD)
Load(C4, P2, ORD)
Fly(P2, ORD, SFO)
Unload(C4, P2, SFO)
Load(C1, P1, SFO)
Fly(P1, SFO, ATL)
Load(C3, P1, ATL)
Fly(P1, ATL, JFK)
Unload(C3, P1, JFK)
Unload(C2, P2, SFO)
Unload(C1, P1, JFK)
```

## 10. A* search with levelsum heuristic function
### Air Cargo Problem 1
 - Expansions: 7
 - Goal Tests: 9
 - New Nodes: 28
 - Plan length: 6
 - Execution time: 0.9002755659894319 seconds
```
Load(C1, P1, SFO)
Load(C2, P2, JFK)
Fly(P1, SFO, JFK)
Fly(P2, JFK, SFO)
Unload(C1, P1, JFK)
Unload(C2, P2, SFO)
```

### Air Cargo Problem 2
 - Expansions: 77
 - Goal Tests: 79
 - New Nodes: 760
 - Plan length: 9
 - Execution time: 129.23260724698775 seconds
```
Load(C1, P1, SFO)
Fly(P1, SFO, JFK)
Load(C2, P2, JFK)
Fly(P2, JFK, SFO)
Load(C3, P3, ATL)
Fly(P3, ATL, SFO)
Unload(C3, P3, SFO)
Unload(C2, P2, SFO)
Unload(C1, P1, JFK)
```

### Air Cargo Problem 3
Does not terminate in 10 minutes.
