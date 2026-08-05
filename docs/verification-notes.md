# Verification Notes

## Artifact checks

- Both preserved submission PDFs were opened successfully.
- Page counts were confirmed: five pages for the signed-adder report and four pages for the counter report.
- Text extraction confirmed that each report contains its Verilog design, testbench, and simulation-results section.
- Visual rendering confirmed that the adder report includes a GTKWave result image and the counter report includes a waveform showing the decimal count sequence.
- SHA-256 hashes were calculated after copying and compared with the uploaded originals.

## What was not performed

A fresh Verilog compilation or simulation was not performed because the upload contains source listings only inside PDF reports. The repository does not silently reconstruct executable `.v` files from those reports.
