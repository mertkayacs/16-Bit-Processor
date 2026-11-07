<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="docs/brand/svg/16-bit-processor-logo-on-dark.svg">
    <img src="docs/brand/svg/16-bit-processor-logo-on-light.svg" alt="16-Bit Processor" width="260">
  </picture>
</p>

<h1 align="center">A 16-bit CPU in Verilog. One instruction per cycle.</h1>

<p align="center">
  Coursework from 2019: a 16-bit processor with a self-checking testbench.<br>
  <b>16 registers. 8 opcodes. Simulated with Icarus Verilog.</b>
</p>

<p align="center">
  <img alt="Language: Verilog" src="https://img.shields.io/badge/language-Verilog-2F6B5B?style=flat-square">
  <img alt="Simulator: Icarus Verilog" src="https://img.shields.io/badge/simulator-Icarus%20Verilog-2F6B5B?style=flat-square">
  <img alt="16 general-purpose registers" src="https://img.shields.io/badge/registers-16-2F6B4F?style=flat-square">
  <img alt="Coursework, 2019" src="https://img.shields.io/badge/project-coursework%202019-2F6B5B?style=flat-square">
  <a href="https://github.com/mertkayacs/16-Bit-Processor"><img alt="GitHub stars" src="https://img.shields.io/github/stars/mertkayacs/16-Bit-Processor?style=flat-square&logo=github&color=8A6D3B"></a>
</p>

<p align="center">
  <a href="#quick-start"><img alt="Quick start" src="https://img.shields.io/badge/Quick%20start-2F6B5B?style=for-the-badge&logo=data%3Aimage%2Fsvg%2Bxml%3Bbase64%2CPHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgd2lkdGg9IjI0IiBoZWlnaHQ9IjI0Ij48ZyBmaWxsPSJub25lIiBzdHJva2U9IiNmZmZmZmYiIHN0cm9rZS1saW5lY2FwPSJyb3VuZCIgc3Ryb2tlLWxpbmVqb2luPSJyb3VuZCIgc3Ryb2tlLXdpZHRoPSIyIj48cGF0aCBkPSJNMTIgMTV2NXMzLjAzLS41NSA0LTJjMS4wOC0xLjYyIDAtNSAwLTUiLz48cGF0aCBkPSJNNC41IDE2LjVjLTEuNSAxLjI2LTIgNS0yIDVzMy43NC0uNSA1LTJjLjcxLS44NC43LTIuMTMtLjA5LTIuOTFhMi4xOCAyLjE4IDAgMCAwLTIuOTEtLjA5Ii8%2BPHBhdGggZD0iTTkgMTJhMjIgMjIgMCAwIDEgMi0zLjk1QTEyLjg4IDEyLjg4IDAgMCAxIDIyIDJjMCAyLjcyLS43OCA3LjUtNiAxMWEyMi40IDIyLjQgMCAwIDEtNCAyeiIvPjxwYXRoIGQ9Ik05IDEySDRzLjU1LTMuMDMgMi00YzEuNjItMS4wOCA1IC4wNSA1IC4wNSIvPjwvZz48L3N2Zz4%3D&logoColor=white"></a>
  <a href="islemci.v"><img alt="Processor" src="https://img.shields.io/badge/Processor-1E2A38?style=for-the-badge&logo=data%3Aimage%2Fsvg%2Bxml%3Bbase64%2CPHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgd2lkdGg9IjI0IiBoZWlnaHQ9IjI0Ij48ZyBmaWxsPSJub25lIiBzdHJva2U9IiNmZmZmZmYiIHN0cm9rZS1saW5lY2FwPSJyb3VuZCIgc3Ryb2tlLWxpbmVqb2luPSJyb3VuZCIgc3Ryb2tlLXdpZHRoPSIyIj48cGF0aCBkPSJNMTIgMjB2MiIvPjxwYXRoIGQ9Ik0xMiAydjIiLz48cGF0aCBkPSJNMTcgMjB2MiIvPjxwYXRoIGQ9Ik0xNyAydjIiLz48cGF0aCBkPSJNMiAxMmgyIi8%2BPHBhdGggZD0iTTIgMTdoMiIvPjxwYXRoIGQ9Ik0yIDdoMiIvPjxwYXRoIGQ9Ik0yMCAxMmgyIi8%2BPHBhdGggZD0iTTIwIDE3aDIiLz48cGF0aCBkPSJNMjAgN2gyIi8%2BPHBhdGggZD0iTTcgMjB2MiIvPjxwYXRoIGQ9Ik03IDJ2MiIvPjxyZWN0IHg9IjQiIHk9IjQiIHdpZHRoPSIxNiIgaGVpZ2h0PSIxNiIgcng9IjIiLz48cmVjdCB4PSI4IiB5PSI4IiB3aWR0aD0iOCIgaGVpZ2h0PSI4IiByeD0iMSIvPjwvZz48L3N2Zz4%3D&logoColor=white"></a>
  <a href="islemci_tb.v"><img alt="Testbench" src="https://img.shields.io/badge/Testbench-1E2A38?style=for-the-badge&logo=data%3Aimage%2Fsvg%2Bxml%3Bbase64%2CPHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgd2lkdGg9IjI0IiBoZWlnaHQ9IjI0Ij48ZyBmaWxsPSJub25lIiBzdHJva2U9IiNmZmZmZmYiIHN0cm9rZS1saW5lY2FwPSJyb3VuZCIgc3Ryb2tlLWxpbmVqb2luPSJyb3VuZCIgc3Ryb2tlLXdpZHRoPSIyIj48cGF0aCBkPSJNMTQgMnY2YTIgMiAwIDAgMCAuMjQ1Ljk2bDUuNTEgMTAuMDhBMiAyIDAgMCAxIDE4IDIySDZhMiAyIDAgMCAxLTEuNzU1LTIuOTZsNS41MS0xMC4wOEEyIDIgMCAwIDAgMTAgOFYyIi8%2BPHBhdGggZD0iTTYuNDUzIDE1aDExLjA5NCIvPjxwYXRoIGQ9Ik04LjUgMmg3Ii8%2BPC9nPjwvc3ZnPg%3D%3D&logoColor=white"></a>
</p>

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="docs/assets/readme/hero-dark.webp">
    <img src="docs/assets/readme/hero-light.webp" alt="Terminal showing the Icarus Verilog compile and run of the 16-bit processor testbench, ending with the line SUCCESS" width="960">
  </picture>
</p>

16-Bit Processor is a processor written in Verilog for a university course in 2019. It runs one instruction per clock cycle and has 16 general-purpose registers, a special function register, a unified 64 KB instruction and data memory, and an eight-opcode instruction set. A testbench loads a program from Mem.mem, runs it and checks the result.

---

## Why 16-Bit Processor

The design is small enough to read in one sitting.

|  |  |
|---|---|
| <img src="docs/assets/readme/icons/cpu.svg" width="18" height="18" alt=""> **One instruction per cycle** | Fetch, decode and execute happen in a single clock cycle, as the repository description states. |
| <img src="docs/assets/readme/icons/binary.svg" width="18" height="18" alt=""> **Small instruction set** | Eight opcodes, with 9-bit and 13-bit immediates extended to 16 bits by [Extender.v](Extender.v). |
| <img src="docs/assets/readme/icons/layers.svg" width="18" height="18" alt=""> **Five modules** | The processor, the ALU, the extender, the unified memory and the shifter each have their own file. |
| <img src="docs/assets/readme/icons/circle-check.svg" width="18" height="18" alt=""> **A testbench that checks itself** | The testbench runs the program in Mem.mem and prints SUCCESS when register 6 holds 0x004c. |

## Features

**Processor**

- 16 general-purpose registers and a special function register, SFR_A.
- Byte-addressed unified memory for instructions and data, 16-bit addresses.
- ALU with add, subtract and equality, and a shifter that shifts left or right by the amount in SFR_A.

**Test**

- Program image in Mem.mem, one byte per line, loaded with $readmemb.
- Testbench reports SUCCESS or a failure message.

## Quick start

```sh
iverilog -o islemci_tb islemci_tb.v islemci.v AMB.v Extender.v Memory.v Shifter.v
vvp islemci_tb
```

The run prints a `$readmemb` warning from the simulator and then `SUCCESS !!`. The testbench has no `$finish`, so stop the simulation with Ctrl+C after the result prints.

### Requirements

- Icarus Verilog (iverilog and vvp).

## Modules

| File | Role |
|---|---|
| `islemci.v` | The processor: fetch, decode and execute. |
| `AMB.v` | Arithmetic logic unit: add, subtract, equality. |
| `Extender.v` | Sign or zero extension of 9-bit and 13-bit immediates. |
| `Memory.v` | Unified byte-addressed memory. |
| `Shifter.v` | Shift left or right by SFR_A. |
| `Mem.mem` | Program image in binary, one byte per line. |

## FAQ

<details>
<summary><b>Which simulator do I need?</b></summary>

Icarus Verilog. The two commands above compile and run the testbench.
</details>

<details>
<summary><b>How do I know it works?</b></summary>

The testbench prints SUCCESS when register 6 holds 0x004c after the program in Mem.mem finishes.
</details>

<details>
<summary><b>Why does the simulation not stop?</b></summary>

The clock in the testbench runs forever and there is no $finish. Press Ctrl+C after the result.
</details>

<details>
<summary><b>Why are the names Turkish?</b></summary>

The course was taught in Turkish. islemci means processor, and the opcode names in islemci.v are Turkish abbreviations.
</details>

If 16-Bit Processor is useful to you, a ⭐ helps other people find it.

Photos behind the screenshots are credited in [docs/assets/readme/CREDITS.md](docs/assets/readme/CREDITS.md).

[![views](https://hits.sh/github.com/mertkayacs/16-Bit-Processor.svg?view=today-total&style=flat-square&label=views&color=2F6B5B&labelColor=1E2A38)](https://github.com/mertkayacs/16-Bit-Processor)
