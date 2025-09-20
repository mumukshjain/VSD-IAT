Summary of Chip Design Flow:

1. **Chip Modelling (O1):**
   - Specifications written in C (high-level model).
   - Testbench is also written in C.
   
2. **RTL Architect (O2):**
   - Hardware is described using RTL (Verilog).
   - Contains processor, peripherals/IPs.
   - Output: Gate-level netlist (Synth P1), macros (synthesized RTL), and 
analog IPs.
   
3. **SoC Integration (O3):**
   - Integration of processor, macros, and analog IPs with GPIOs.
   - Floorplanning, placement, CTS, routing.
   - RTL2GDS stage.
   
4. **Final Stage:**
   - GDSII file generated.
   - DRC/LVS checks performed.
   - Sent for fabrication.

This workflow shows the transition from **specifications → RTL → 
synthesis → physical design → tape-out**.
