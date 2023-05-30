# 16:1  MULTIPLEXER  USING VERILOG

## AIM :
   To implement 16:1  multiplexer using verilog and validate its outputs
   
## HARDWARE REQUIRED : 
   – PC, Cyclone II , USB flasher  
   
## SOFTWARE REQUIRED:
   Quartus prime  
   
## THEORY :   

### What is a Multiplexer ?
    
  The multiplexer is a device that has multiple inputs and single line output. The select lines determine which input is connected to the output, and also increase the amount of data that can be sent over a network within a certain time. It is also called a data selector.

  The single-pole multi-position switch is a simple example of a non-electronic circuit of the multiplexer, and it is widely used in many electronic circuits. The multiplexer is used to perform high-speed switching and is constructed by electronic components.
  
  
  ![image](https://github.com/Jayabharathi3/Simulation-project--Digital-Electronics/assets/120367796/1194d84e-6da0-464d-88ed-3e999ef33d28)
  
  
  
### 16 to 1 Multiplexer

   In the 16 to 1 multiplexer, there are total of 16 inputs, i.e., A0, A1, …, A16, 4 selection lines, i.e., S0, S1, S2, and S3 and single output, i.e., Y. On the basis of the combination of inputs that are present at the selection lines S0, S1, and S2, one of these 16 inputs will be connected to the output. The block diagram and the truth table of the 16×1
   
   A 16:1 multiplexer is a digital logic component that has 16 input lines, one output line, and four control or select lines. It is also known as a 16-input multiplexer. The select lines determine which input line is connected to the output line.

The control or select lines are usually binary and represent a unique combination of values from 0 to 15 (in binary form). Each combination of select line values corresponds to one of the 16 input lines. The selected input line is then routed to the output line.
  
  
  In the truth table above, S3, S2, S1, and S0 represent the four select lines, and I15 to I0 represent the input lines. The selected input line, determined by the select lines' binary combination, is passed to the output line.

The 16:1 multiplexer is often used in digital systems to select one out of 16 inputs and route it to the output based on the control signals provided by the select lines.
 


   ![16 mux](https://github.com/Jayabharathi3/Simulation-project--Digital-Electronics/assets/120367796/626b76cb-d667-406f-a095-8c7cfd9e913b)
   
   
   
# PROCEDURE  

## Step 1
Create a project with required entities.

## Step 2
Create a module along with file name for both Multiplexer .

## Step 3
Run the module and get the respective RTL outputs.

## Step 4
Create university program(VWF) for getting timing diagram.

## Step 5
Give the respective inputs for timing diagram and obtain the results.

        
# PROGRAM  

```
/*
Program for flipflops  and verify its truth table in quartus using Verilog programming.
Developed by: JAYABHARATHI.S
RegisterNumber: 212222100013 
*/

module muux (out,a,s);
input[15:0]a;
input[3:0]s;
output reg out;
always@(a,s)
begin
case(s)
4'b0000:out=a[0];
4'b0001:out=a[1];
4'b0010:out=a[2];
4'b0011:out=a[3];
4'b0100:out=a[4];
4'b0101:out=a[5];
4'b0110:out=a[6];
4'b0111:out=a[7];
4'b1000:out=a[8];
4'b1001:out=a[9];
4'b1010:out=a[10];
4'b1011:out=a[11];
4'b1100:out=a[12];
4'b1101:out=a[13];
4'b1110:out=a[14];
4'b1111:out=a[15];
endcase
end
endmodule



```
# LOGIC DIAGRAM  (REFERENCE)

![image](https://github.com/Jayabharathi3/Simulation-project--Digital-Electronics/assets/120367796/e37d33f2-5be7-4073-8027-62f364fb12d3)


# NETLIST DIAGRAM

![stprrtl](https://github.com/Jayabharathi3/Simulation-project--Digital-Electronics/assets/120367796/d2dcdbfb-61b2-4fdd-870d-6d5370e4d27c)


![muxrtl16](https://github.com/Jayabharathi3/Simulation-project--Digital-Electronics/assets/120367796/a9bd3e79-e316-453a-9c03-6d51287f0021)


# TIMING DIAGRAM


![muxtt16](https://github.com/Jayabharathi3/Simulation-project--Digital-Electronics/assets/120367796/0a63af42-84da-4f5a-87a6-23425154dc3b)



# TRUTH TABLE


![image](https://github.com/Jayabharathi3/Simulation-project--Digital-Electronics/assets/120367796/94575ee8-ae67-402d-9c22-a3f204a453a3)


# RESULT

Thus the implementation of  16 : 1 Multiplexer are verified

