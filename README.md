# Verilog RTL Design and Simulation

A preserved portfolio of two Verilog logic-design exercises covering **hierarchical combinational arithmetic** and **clocked sequential control**.

The repository contains the original submitted PDF reports without modifying their contents. The surrounding documentation was added to make the designs easier to review as a technical portfolio.

## Projects

### 1. 8-bit signed ripple-carry adder

A gate-level two's-complement adder built hierarchically from half-adder and full-adder modules. Eight full-adder stages form the ripple path, and signed overflow is detected by comparing the carry entering and leaving the most-significant bit.

Key topics:

- structural Verilog;
- hierarchical module composition;
- ripple-carry propagation;
- signed two's-complement arithmetic;
- overflow and underflow detection; and
- waveform-based verification.

[Open project documentation](projects/signed-ripple-carry-adder/README.md)

### 2. Triggered decimal counter

A 4-bit sequential design that enters a counting state after a qualifying input pattern, advances through decimal values, and returns to zero after reaching nine. The implementation also includes asynchronous active-low reset behavior and a testbench that generates VCD output.

Key topics:

- sequential Verilog;
- state held in registers;
- clocked and asynchronous-reset behavior;
- finite-state control using flags;
- testbench stimulus sequences; and
- waveform inspection.

[Open project documentation](projects/triggered-decimal-counter/README.md)

## Repository structure

```text
verilog-rtl-designs/
├── README.md
├── ORIGINAL_FILE_MANIFEST.tsv
├── SOURCE_PRESERVATION.md
├── PRIVACY_NOTE.md
├── docs/
│   ├── portfolio-scope.md
│   └── verification-notes.md
└── projects/
    ├── signed-ripple-carry-adder/
    │   ├── README.md
    │   ├── media/
    │   │   └── simulation-waveform.png
    │   └── original/
    │       └── 8-bit-signed-ripple-carry-adder-report.pdf
    └── triggered-decimal-counter/
        ├── README.md
        ├── media/
        │   └── simulation-waveform.png
        └── original/
            └── triggered-decimal-counter-report.pdf
```

## How to review the work

1. Read each project README for a concise architecture and verification summary.
2. Open the preserved PDF report for the complete submitted Verilog listing, testbench, and original simulation evidence.
3. Use `ORIGINAL_FILE_MANIFEST.tsv` to verify that the included reports are byte-for-byte identical to the uploaded files.

## Academic context

These designs originated in an introductory logic-design course. They are presented here as preserved evidence of early RTL design practice rather than as production-ready IP cores. The repository intentionally distinguishes the original work from the later portfolio documentation.

## Important limitation

The original upload contains the Verilog listings inside PDF reports rather than separate `.v` files. No source code was transcribed, rewritten, corrected, or reconstructed for this repository because doing so would no longer preserve the submitted artifacts exactly.
