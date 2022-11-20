# Uint-Packing

## Introduction

DSP blocks are undoubtedly efficient solutions for implementing multiply-accumulate (MAC) operations on FPGA. Since DSP resources are scarce in FPGA, the advanced solution is to pack parallel multiplication operations into a single DSP. However, available methods are based on signed-type multiplication, leading to both loss of accuracy and increased area. To solve these issues simultaneously, we propose an unsigned integer DSP packing generalization model called uint-packing. Guided by this generalization model, we design the novel computational structure of the DNN accelerator.

## Build the Project

1. **Generate HLS project by running:**

   ```shell
   cd ./scripts
   vivado_hls hls_script.tcl
   ```

2. **Generate Vivado project by running:**

   ```shell
   vivado -mode tcl -source rtl_script.tcl
   ```
