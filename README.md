SIMULATION AND IMPLEMENTATION OF MULTIPLIER
**AIM: **
 To simulate and synthesis multiplier using Xilinx ISE.

**APPARATUS REQUIRED:**
Xilinx 14.7
Spartan6 FPGA
  
**PROCEDURE:**
STEP:1  Start  the Xilinx navigator, Select and Name the New project.
STEP:2  Select the device family, device, package and speed.       
STEP:3  Select new source in the New Project and select Verilog Module as the Source type.                       
STEP:4  Type the File Name and Click Next and then finish button. Type the code and save it.
STEP:5  Select the Behavioral Simulation in the Source Window and click the check syntax.                       
STEP:6  Click the simulation to simulate the program and  give the inputs and verify the outputs as per the truth table.               
STEP:7  Select the Implementation in the Sources Window and select the required file in the Processes Window.
STEP:8  Select Check Syntax from the Synthesize  XST Process. Double Click in the  FloorplanArea/IO/Logic-Post Synthesis process in the User Constraints process group. UCF(User constraint File) is obtained. 
STEP:9  In the Design Object List Window, enter the pin location for each pin in the Loc column Select save from the File menu.
STEP:10 Double click on the Implement Design and double click on the Generate Programming File to create a bitstream of the design.(.v) file is converted into .bit file here.
STEP:11  On the board, by giving required input, the LEDs starts to glow light, indicating the output.

**Logic Diagram**
2 bit Multiplier

![image](https://github.com/navaneethans/VLSI-LAB-EXP-3/assets/6987778/7713750f-65e6-41c0-8082-5005eac4031c)

**4 Bit Multiplier**

![image](https://github.com/navaneethans/VLSI-LAB-EXP-3/assets/6987778/d95215dd-8cf1-4e08-93cc-96adfdd7fbdc)


**Verilog code**

3_MULTIPLIER_2BIT:
~~~
module ha(a,b,sum,carry);
input a,b;
output sum,carry;

endmodule

module multi_2(a,b,p,carry);
input [1:0]a,b;
output [2:0]p;
output carry;

endmodule
~~~

OUTPUT:







3_MULTIPLIER_4BIT:
~~~
module ha(a,b,sum,carry);
input a,b;
output sum,carry;
endmodule

module fa_ha(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
endmodule

module multi_4(a,b,p,carry);
input[3:0]a,b;
output [6:0]p;
output carry;
wire [17:1]w;
endmodule
~~~

OUTPUT:









RESULT:






