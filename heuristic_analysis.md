## Breadth first search
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
TODO:

### Air Cargo Problem 3
TODO:

## A* search with h_ignore_preconditions
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