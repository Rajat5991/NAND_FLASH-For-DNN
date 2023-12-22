# NAND_FLASH - A Potential Contender for DNN
Traditional computing systems Fig.1 typically store massive information on a memory unit that is physically connected to the computational unit by a data bus. The continuous data movement between the processing and the memory units represents the main bottleneck due to the limited bandwidth, long latency, sequential data processing, and high energy consumption. To minimize the latency and energy overhead of conventional von Neumann computers, in-memory computing (IMC) aims at performing the computation within the memory.

<img width="549" alt="image" src="https://github.com/Rajat5991/NAND_FLASH-For-In-Memory-Computing/assets/154459536/09cc09e0-4196-4019-b842-506299999405">

# NAND_FLASH Background 

NAND flash array consists of multiple blocks, and each block consists of multiple strings as shown in Figs. 2a and 2b. Strings in NAND flash are connected via a shared bitline. Each string contains a series of floating gate cells in Fig. 2b, so one current value flows through the NAND string for the read operation. To read the stored data in the NAND flash array, it first selects the block that contains the target cell using block select transistors: SSL & GSL. The block select transistors in the selected block are applied Vpass, which is larger than V th, to flow the current through the block in Fig. 2d. Second, the unselected cells in the selected block are also applied Vpass to flow the current through the block regardless of the stored data of the unselected cells. Vread applies to the selected cell for the read operation. NAND flash distinguishes the stored data by the threshold voltage of a floating gate cell as shown in Fig. 2c. When the stored data is ”1”, the threshold voltage of the cell
is lower than the read voltage Vread, so the cell produces the current. However, if the stored data is ”0”, the threshold voltage of the cell is higher than the Vread. In this case, the current does not flow through the cell. Therefore, the string can produce the current depending on the stored data, and NAND flash can read the stored data of the selected page by sensing the current from the shared bit-line.

<img width="420" alt="image" src="https://github.com/Rajat5991/NAND_FLASH-For-In-Memory-Computing/assets/154459536/0a755689-cdcb-4d2c-be54-f27d6da90160">
                                                           Fig.2 NAND_FLASH

