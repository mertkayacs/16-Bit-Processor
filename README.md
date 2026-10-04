# 16-Bit-Processor

A 16-bit processor written in Verilog, one instruction per cycle. It has 16 general purpose registers, a special function register (SFR_A), a unified 64 KB instruction and data memory, and an 8 opcode instruction set. A testbench runs a program loaded from `Mem.mem` and checks the result.

## How to run

You need Icarus Verilog (`iverilog`). From the repo root:

```
iverilog -o islemci_tb islemci_tb.v islemci.v AMB.v Extender.v Memory.v Shifter.v
vvp islemci_tb
```

The testbench (`islemci_tb.v`) loads the program from `Mem.mem` into memory, runs it, and prints `SUCCESS !!` if register 6 holds the expected value. The testbench has no `$finish`, so stop the simulation with Ctrl+C after the result prints.

## Modules

- `islemci.v`: the processor. Fetches, decodes, and executes instructions.
- `AMB.v`: arithmetic logic unit (add, subtract, equality).
- `Extender.v`: sign or zero extends 9-bit and 13-bit immediates to 16 bits.
- `Memory.v`: unified byte addressed memory for instructions and data.
- `Shifter.v`: shifts a register left or right by the amount in SFR_A.
- `Mem.mem`: memory image in binary, one byte per line, loaded with `$readmemb`.

## Tech used

- Verilog
- Icarus Verilog (simulation)

## Status

Coursework, 2019 (committed 2020).
