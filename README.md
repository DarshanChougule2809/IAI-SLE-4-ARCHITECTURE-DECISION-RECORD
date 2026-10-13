# IAI-SLE-4-ARCHITECTURE-DECISION-RECORD


## Project Title
**Performance Comparison of BFS and DFS on a 20 × 20 Grid**

**Course:** 02AML204 – Introduction to Artificial Intelligence  
**Student:** Darshan Jivandhar Chougoule  
**PRN:** 25UAM077  
**Division:** B  
**Submission Date:** 11 October 2026

## Overview
SLE-4 documents the technical decision to use Breadth-First Search (BFS) as the reference algorithm for shortest-path finding in an unweighted 20 × 20 grid. Depth-First Search (DFS) is retained as a comparison algorithm.

The search starts at `(0, 0)` and targets `(19, 19)`. The project compares path length, number of expanded nodes, and execution time.

## Decision Summary
- **Selected reference algorithm:** BFS
- **Comparison algorithm:** DFS
- **Reason:** BFS explores level by level and guarantees a shortest path in an unweighted grid.
- **Trade-off:** BFS can use more memory because it stores frontier nodes. DFS may sometimes reach the goal quickly, but it does not guarantee the shortest path.
- **Scope:** This decision applies to unweighted grids. Weighted path costs may require a different algorithm.

## Main Concepts
- **Queue (FIFO):** Used by BFS to process cells in discovery order.
- **Stack (LIFO):** Used by DFS to explore one branch deeply before backtracking.
- **Visited set:** Prevents repeated exploration of cells and helps avoid cycles.
- **Parent map:** Stores predecessor information so the final path can be reconstructed.
- **Profiling:** Measures path length, expanded nodes, and execution time across repeated runs.

## SLE Journey
1. **SLE-1 – Study Assistant AI Agent:** A Python menu-based study assistant with percentage calculation, study tips, a basic calculator, and exit.
2. **SLE-2 – Empirical Performance Analysis:** Compared BFS and DFS on a 20 × 20 grid using path length, expanded nodes, and repeated execution-time measurements.
3. **SLE-3 – BFS vs DFS Grid Search and C4 Architecture:** Documented the system architecture by separating grid configuration, neighbor validation, search engines, profiler, and output.
4. **SLE-4 – ADR Defense:** Recorded and justified BFS as the reference for shortest-path finding on an unweighted grid while retaining DFS for comparison.

## Project Structure
The architecture described in SLE-3 separates responsibilities into modules such as:
- Grid configuration
- Valid-neighbor checking
- BFS search
- DFS search
- Performance profiling
- Output/reporting

> Adapt this section if the actual repository uses different filenames or folders.

## Running and Verifying
Use the run instructions and commands provided in the source code repository for SLE-1, SLE-2, and SLE-3. Run the profiler before reporting performance results.

**Important:** Exact timing values are not included in the SLE-4 document. Copy measured values from your actual program output; do not estimate or invent them.

## Expected Viva Points
- BFS guarantees the shortest path in an unweighted grid.
- DFS does not guarantee the shortest path.
- The visited set prevents revisiting cells.
- The parent map supports path reconstruction.
- Profiling compares path length, expanded nodes, and execution time.
- BFS can require more memory on larger grids.

## AI Contribution and Academic Responsibility
ChatGPT was used to help organize the ADR, improve clarity, and prepare possible viva explanations. The student is responsible for understanding the code, checking this README against the actual implementation, running the profiler, verifying measurements, and explaining the decision during the viva.

## Related Repositories
- SLE-1 – Study Assistant AI Agent: https://github.com/DarshanChougule2809/IAI-SLE-AI-Agent
- SLE-2 – Empirical Performance Analysis: https://github.com/DarshanChougule2809/IAI-SLE-2-profiling
- SLE-3 – BFS vs DFS Grid Search and C4 Architecture: https://github.com/DarshanChougule2809/IAI-SLE-3-Architecture
