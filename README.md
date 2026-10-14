# otimizacao-trab2-
Second assignment of CI1238 Optimization (UFPR): solve the **"Comissão Representativa"** (representative committee) problem with **Branch & Bound**.

**Problem.** Given a set of groups *S* and candidates *C*, where each candidate belongs to some groups, pick the smallest set of candidates so that every group is represented (a minimum set cover). If no selection covers all groups the program prints `Inviavel`.

**Implementation (`trab2.py`).** Branch & Bound over include/exclude decisions for each candidate, with feasibility cuts, optimality cuts and a bounding function. Command-line options:
- `-a` use the bounding function given by the professor (|E| + 1 while some group is uncovered); by default a tighter bound of my own is used
- `-f` disable feasibility cuts
- `-o` disable optimality cuts

Input is read from `stdin` (|S| and |C|, then one block per candidate listing its groups) and the chosen candidates are printed in ascending order, after a short report with the elapsed time and the number of tree nodes explored. `entradas_avaliadas/` has the instances used to compare the bounding functions (tree nodes and time).
