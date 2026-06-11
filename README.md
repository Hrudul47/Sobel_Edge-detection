# FPGA-Based Edge Detection (Sobel Hardware Implementation)

## 📌 Overview

This project presents the implementation of the **Sobel Edge Detection** algorithm on FPGA hardware using Verilog HDL for real-time image processing.

The system processes grayscale images with a resolution of **128 × 128 pixels (16,384 pixels total)** and generates edge-detected output suitable for display through a VGA interface.

---

## 🔹 Sobel Edge Detection (Hardware Implementation)

### ⚙️ Description

The Sobel operator is implemented as a fully functional FPGA design using Verilog HDL. It computes horizontal and vertical image gradients using fixed 3×3 convolution kernels and generates edge-detected output in real time.

### 🏗️ Key Features

* Real-time edge detection on FPGA
* Fully pipelined architecture
* VGA display output support
* Modular Verilog design
* Efficient hardware resource utilization
* Suitable for image processing applications

### 🛠️ Hardware Platform

* FPGA Board: Nexys A7
* FPGA Device: Xilinx Artix-7 XC7A100T
* Development Tool: Xilinx Vivado

### 📁 Project Structure

```text
sobel.v
sobel_edge.v
edge_top.v
edge_controller.v
line_buffer.v
window3x3.v
input_frame_buffer.v
output_frame_buffer.v
vga_display.v
vga_sync.v
constraint.xdc
edge_tb.v
```

### ▶️ Implementation Steps

1. Open Xilinx Vivado.
2. Create a new RTL project.
3. Add all Sobel-related Verilog source files.
4. Add the constraint file (`constraint.xdc`).
5. Run Synthesis.
6. Run Implementation.
7. Generate Bitstream.
8. Program the Nexys A7 FPGA board.
9. Connect a VGA monitor and observe the edge-detected output.

### 📊 Sobel Results

| Parameter        | Value     |
| ---------------- | --------- |
| Image Resolution | 128 × 128 |
| Total Pixels     | 16,384    |
| Edge Pixels      | 4,820     |
| Edge Density     | 29.41%    |

#### Observation

The Sobel operator successfully detects major image edges and provides real-time performance. However, due to its first-order gradient nature, the output may contain noise and thick edges.

---

## 🚀 Applications

* Real-time video processing
* Computer vision systems
* Autonomous vehicles
* Object detection
* Medical image analysis
* Surveillance systems

---

## 🧑‍💻 Author

**Hrudul S**

B.Tech Electronics and Communication Engineering

Interested in FPGA Design, Digital VLSI, RTL Design, and Embedded Image Processing.

---

## 📜 License

This project is intended for academic and research purposes.
