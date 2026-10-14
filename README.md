# otimizacao-trab2-
Assignment 2 for Optimization (BCC, UFPR): a **branch-and-bound** solver in Python (`trab2.py`) for a combinatorial selection problem — choose the smallest number of items whose sets cover the required elements.

The search includes a bounding function and pruning by optimality and by feasibility. Command-line flags:
- `-a` use the default (simple) bounding function
- `-o` disable optimality cuts
- `-f` disable feasibility cuts

`entradas_avaliadas/` contains the evaluated input instances and sample outputs.
