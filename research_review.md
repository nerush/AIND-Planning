# Research Review by Yevgen Nerush

Automated planning and scheduling (1), sometimes denoted as planning, is the
branch of artificial intelligence that concerns the realization of strategies
of action sequence, typically for execution by intelligent agents, autonomous robots
and unmanned vehicles. In order to describe how actions affect the states
of systems over time, an action language is commonly used in the
artificial intelligence and robotics domains.

Action languages fall into two classes: action description languages and action query languages.
Examples of the former include STRIPS (Stanford Research Institute Problem Solver) (3), ADL and PDDL.
STRIPS is the base for most of the languages for expressing automated planning problem instances
in use today. It is an automated planning technique that works by executing a domain and problem
to find a goal. With STRIPS, you first describe the world. You do this by providing objects,
actions, preconditions, and effects. It is used in a deterministic world only and is not complete.
It cannot solve some very simple problems, such as the Sussman anomaly,
found by Allen Brown during experimentation with the HACKER system.
One solution to the interleaving problem was goal-regression planning,
which was introduced by Waldinger in his WARPLAN planner.

Currently the most popular and effective approaches to fully automated planning are:
 - Translating to a Boolean satisfiability (SAT) problem
 - Forward state-space search with carefully crafted heuristics
 - Search using a planning graph, called GRAPHPLAN (4)


Planners such as GRAPHPLAN, SATPLAN, and FF have moved the field of planning forward,
by raising the level of performance of planning systems, by clarifying the representational
and combinatorial issues involved, and by the development of useful heuristics.
However, there is a question of how far these techniques will scale. It seems
likely that further progress on larger problems cannot rely only on factored and
propositional representations, and will require some kind of synthesis of first-order
and hierarchical representations with the efficient heuristics currently in use. (5)



1. [Automated planning and scheduling on Wikipedia](https://en.wikipedia.org/wiki/Automated_planning_and_scheduling)
2. [Action language on Wikipedia](https://en.wikipedia.org/wiki/Action_language)
3. [Richard E. Fikes, Nils J. NHsson. STRIPS: A New Approach to the Application of .Theorem Proving toProblem Solving'](http://ai.stanford.edu/~nilsson/OnlinePubs-Nils/PublishedPapers/strips.pdf)
4. [Avrim L. Blum, Merrick L. Furst. Fast Planning Through Planning Graph Analysis](https://www.cs.cmu.edu/~avrim/Papers/graphplan.pdf)
5. Stuart Russel, Peter Norvig. Artificial Intelligence, A Modern Approach, Third Edition
