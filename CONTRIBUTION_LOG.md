# SLE-4 Contribution Log

**Project:** Performance Comparison of BFS and DFS on a 20 × 20 Grid  
**Course:** 02AML204 – Introduction to Artificial Intelligence  
**Student:** Darshan Jivandhar Chougoule  
**PRN:** 25UAM077  
**Division:** B

## Contribution Summary

| No. | Task | Contribution / Evidence |
|---:|---|---|
| 1 | Review previous SLE work | Connected the SLE-1 Study Assistant, SLE-2 profiling, and SLE-3 architecture work in the SLE journey summary. |
| 2 | Define the decision | Documented BFS as the reference algorithm for shortest-path finding on an unweighted grid. |
| 3 | Compare alternatives | Summarized DFS and the option of using only BFS; noted A* as a possible alternative for larger pathfinding tasks. |
| 4 | Explain the rationale | Explained BFS level-by-level exploration, FIFO queue, visited set, and parent map; contrasted DFS stack-based exploration. |
| 5 | Record trade-offs | Documented BFS's shortest-path guarantee and higher potential memory use, and DFS's lack of a shortest-path guarantee. |
| 6 | Document profiling | Identified path length, expanded nodes, and execution time as comparison measures. |
| 7 | Prepare for viva | Prepared short explanations of BFS, DFS, visited set, parent map, profiling, and scaling to larger grids. |
| 8 | Prepare documentation | Organized the SLE-4 decision and project summary into the ADR and README. |

## AI Tool Usage
ChatGPT helped organize the ADR, improve wording, and prepare possible viva explanations. The student must verify the documentation against the actual code and perform the profiling.

## Verification Still Required
- [ ] Run the actual project and confirm it uses the documented 20 × 20 grid.
- [ ] Confirm the start is `(0, 0)` and the goal is `(19, 19)`.
- [ ] Verify BFS and DFS outputs against the current code.
- [ ] Run the profiler and record actual timing values and other metrics.
- [ ] Check the repository filenames and update the README's project structure if needed.
- [ ] Ensure the final files reflect the work actually completed by each contributor.

## Accuracy Note
This log records the work described in the SLE-4 document. It does not claim unverified code changes, commits, or exact performance results. Add dates, team members, commit hashes, and individual contributions only when confirmed from the actual repository history.
