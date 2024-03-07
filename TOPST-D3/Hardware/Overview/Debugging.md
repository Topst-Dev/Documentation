<h1>
  Debugging
</h1>


## Debugger I/F Connector (UART/JTAG) to Host PC  

Figure 1.1 shows the 0.5 mm Pitch 20-pin FFC (A side–B side) used for debugging.  
<p align="center"><img src="https://github.com/Topst-Dev/Documentation/assets/161264431/21cef494-2147-4d43-91ca-004d4c8acb16"></p>  


## Debug Port on TOPST D3  

The TOPST D3 uses serial communication for debugging output, and Debug is designed for FFC connector.  

Figure 1.2 shows the appearance of Debug on the TOPST D3.  
<p align="center"><img src="https://github.com/Topst-Dev/Documentation/assets/161264431/490ba306-6322-43f1-9210-581772203890"></p>  


## UART/JTAG Sub-board  

The UART/JTAG sub-board is a debugging board for serial port and JTAG. You can check the serial log by connecting the UART/JTAG sub-board to your Host PC using a USB Type-C cable.   

Figure 1.3 shows the overview of the UART/JTAG sub-board.  
<p align="center"><img src="https://github.com/Topst-Dev/Documentation/assets/161264431/e330d74c-e1a9-45ec-b2a7-c2520ad47e68"></p>  

Table 1 describes the connectors of the UART/JTAG sub-board.  

**Table 1 Description of UART/JTAG Sub-board:**  

| Item | Description                                    |
|:----:|------------------------------------------------|
| u10  | FFC connector to connect the TOPST D3          |
| u20  | Male Pin Header to connect debugger            |
| u30  | Debug port (USB Type-C) for MCU debugging      |
| u40  | Debug port (USB Type-C) for A53 Core debugging |
| u50  | Debug port (USB Type-C) for A72 Core debugging |  


## Connecting UART/JTAG Sub-board to TOPST D3  

This chapter describes how to connect the TOPST D3 and the UART/JTAG sub-board.  

Connect the UART/JTAG sub-board to the TOPST D3 by using a Flexible Flat Cable (FFC) as follows:
>  1. Prepare one FFC and one USB Type-C cable.
>  2. Connect the FFC to Debug I/F connector on the UART/JTAG sub-board and Debug I/F connector on the TOPST D3
>  >  - It is important to connect the blue line of the FFC facing up.
>  3. Connect the UART/JTAG sub-board to your Host PC by using a USB Type-C cable.
>  >  - Refer to Table 1 to select the appropriate UART port according to the target core. For example, A72 UART can be connected to the UART Port of the main core (Cortex-A72 Quad).
>  4. Check the serial log message through the Terminal application on your Host PC

Figure 1.4 shows the location of Debug on the TOPST D3 connected with Debug on the UART/JTAG sub-board.  
<p align="center"><img src="https://github.com/Topst-Dev/Documentation/assets/161264431/dd1cd014-554e-4948-b0d5-bc976853c75f"></p>  

## Connect JTAG Debugger to TOPST D3  

This chapter describes how to connect JTAG debugger to the TOPST D3.  

Connect JTAG debugger to the TOPST D3 as follows:
>  1. Prepare one JTAG debugger.
>  2. Referring to Chapter Connecting UART/JTAG Sub-board to TOPST D3 above, connect the UART/JTAG sub-board to the TOPST D3.
>  3. Connect the JTAG debugger to JTAG Header on the UART/JTAG Sub-board.

Figure 1.5 shows the location of JTAG Header on the UART/JTAG sub-board.  
<p align="center"><img src="https://github.com/Topst-Dev/Documentation/assets/161264431/d4043853-8723-4fe3-9403-2a4fe413564c"></p>  
