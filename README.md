# Parameterized Synchronous FIFO in Verilog

A robust, parameterizable Synchronous First-In-First-Out (FIFO) buffer design implemented in Verilog and verified via EDA Playground. It performs queue management and data streaming under a single clock domain.

## 🚀 Features
* **Parameterization**: Configurable parameters including data width (`DATA_WIDTH`) to handle scalable data payloads.
* **Single-Clock Domain**: Synchronizes both push (write) and pop (read) operations to a common clock (`clk`) with active-low synchronous/asynchronous reset (`rst_n`).
* **Status Flags**: Generates real-time `full` and `empty` indicator flags to prevent buffer overflow and underflow conditions.
* **Testbench Verification**: Accompanied by a structured testbench (`syn_fifo_tb`) featuring automated stimulus queues and clock generation.

## 📂 Project Structure
```text
├── design.sv          # Main Synchronous FIFO RTL module (`synchronous_fifo`)
├── testbench.sv       # Testbench module (`syn_fifo_tb`) for stimulus and monitoring
└── README.md          # Project documentation

🛠️ Simulation & Verification
You can simulate and test this code directly in EDA Playground:

Compile design.sv and testbench.sv.

Run the simulation to observe waveform transitions and self-checking data integrity across write and read sequences.
