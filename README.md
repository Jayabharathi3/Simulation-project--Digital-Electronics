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


module muux(i0,i1,i2,i3,i4,i5,i6,i7,i8,i9,i10,i11,i12,i13,i14,i15,s0,s1,s2,s3,y);
input i0,i1,i2,i3,i4,i5,i6,i7,i8,i9,i10,i11,i12,i13,i14,i15,s0,s1,s2,s3;
output y;
wire a,b,c,d,e,f,g,h,i,j,k,l,m,n,o,p,s0c,s1c,s2c,s3c;
not(s0c,s0);
not(s1c,s1);
not(s2c,s2);
not(s3c,s3);
and(a,s0c,s1c,s2c,s3c,i0);
and(b,s0c,s1c,s2c,s3,i1);
and(c,s0c,s1c,s2,s3c,i2);
and(d,s0c,s1c,s2,s3,i3);
and(e,s0c,s1,s02,s03,i4);
and(f,s0c,s1,s02,s3,i5);
and(g,s0c,s1,s2,s3c,i6);
and(h,s0c,s1,s2,s3,i7);
and(i,s0,s1c,s2c,s3c,i8);
and(j,s0,s1c,s2c,s3,i9);
and(k,s0,s1c,s2,s3c,i10);
and(l,s0,s1c,s2,s3,i11);
and(m,s0,s1,s2c,s3c,i12);
and(n,s0,s1,s2c,s3,i13);
and(o,s0,s1,s2,s3c,i14);
and(p,s0,s1,s2,s3,i15);
or(y,a,b,c,d,e,f,g,h,i,j,k,l,m,n,o,p);
endmodule


```
# LOGIC DIAGRAM

![image](https://github.com/Jayabharathi3/Simulation-project--Digital-Electronics/assets/120367796/e37d33f2-5be7-4073-8027-62f364fb12d3)


# NETLIST DIAGRAM

![stprrtl](https://github.com/Jayabharathi3/Simulation-project--Digital-Electronics/assets/120367796/d2dcdbfb-61b2-4fdd-870d-6d5370e4d27c)


# TIMING DIAGRAM

# TRUTH TABLE


![image](https://github.com/Jayabharathi3/Simulation-project--Digital-Electronics/assets/120367796/94575ee8-ae67-402d-9c22-a3f204a453a3)


# RESULT

Thus the implementation of  16 : 1 Multiplexer are verified


