# NoRFgem5

This is a copy of gem5 modified with TCA instructions. It shows DGEMM instructions using register files and instructions without register files. The register file accesses are split into separate micro-ops for the number of wide loads needed to fill the given size TCA submatrix into a register file. The NoRF instructions issue the loads, do the computation, and stores in a single operation, broken down into several uops. The RF instruction, on the other hand, has separate store instructions, as well as computation instruction.
