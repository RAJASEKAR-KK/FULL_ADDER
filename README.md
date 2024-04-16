# FULL_ADDER
# Aim:
To stimulate and synthesis the Full adder using verilog.

# Apparatus Required:
Vivado Xilinx 14.7 Spartan 6 FPGA.

# Procedure:
```
STEP 1: Start the vivado software and select the name and the project.
STEP 2: Select the device family,device,package and speed.
STEP 3:  Select new source in the new project and select verilog module as the source type.
STEP 4: Type the file name and module name and click next and then finish button. Type the code and save it.
STEP 5: Select the run simulation and then run behavioural simulation in the source window and click the check syntax.
STEP 6: Click the simulation to stimulate the program and give the inputs and verify the outputs as per the truth table.
STEP 7: Compare the output with the truth table.
```
# Truth Table
![image](https://github.com/RESMIRNAIR/FULL_ADDER/assets/154305926/02ead8f5-d958-4c89-ac51-368ca086cf41)
# Circuit Diagram
![image](https://github.com/RESMIRNAIR/FULL_ADDER/assets/154305926/418e00aa-ed19-4ab3-a413-bae9575bff0e)
![image](https://github.com/RESMIRNAIR/FULL_ADDER/assets/154305926/0c26fe47-d78c-43dd-ac0d-804e427a3bbc)
# Program:
```
module FA(a,b,cin,sum,cout);
input a,b,cin;
output sum,cout;
wire w1,w2,w3;
xor g1(w1,a,b);
and g2(w2,w1,cin);
and g3(w3,a,b);
xor g4(sum,w1,cin);
or g5(cout,w2,w3);
endmodule
```
# Output:
![Full Adder](https://github.com/RAJASEKAR-KK/FULL_ADDER/assets/165815233/104cf1bb-6425-475d-ab5c-c6549faf8809)
# Result:
Thus the verilog program for Full Adder has been stimulated and verified successfully.

