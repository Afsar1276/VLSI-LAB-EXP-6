# VLSI-LAB-EXP-6

# SIMULATE AND SYNTHESIS INVERTER USING CADENCE

# AIM:
To create,simulate the design of CMOS inverter,NAND,NOR from schematic using cadence.

# APPARATUS REQUIRED:
cadence

# Commands to get into Cadence

Right Click and open the terminal window Type the following commands as follows and press enter. i) tcsh ii) source /home/install/cshrc iii) virtuoso

# Procedure for Schematic simulation using Cadence

Now two windows must open i)virtuoso/command interpreter window ii)”Whats New…” Close the 2nd window Use 1st window i.e virtuoso window(CIW) for further processing. i) Create a New Library ii) Create Schematic Cell view. iii) Create the Symbol for schematic Cell view. iv) Create the test Cell view. v) Analog simulation by spectre

# Procedure for Creating New Library.
```
a) File –New – Library
b) Name : Give name for ur library Ex: VLSILAB , Enable Attach to an existing technology library, Click OK
c) Attach the library to the technology library gpdk045.Click OK
```
# Create Schematic Cell view.
```
a) Go to 1st window i.e virtuoso(CIW)
b) File-New-Cell view
c) Setup the new file form, Library: Select the one you a created. Cell : Give the experiment name Ex: Inverter View: Schematic
d) Type: Schematic press OK
e) Add the required components from the libraries and make the connections.
f) Go to instance fixed menu or use shortcut key “I” from keypad to go instances Click on browse. This opens the library browser ow select the appropriate library for components like Gpdk045,nmos, pmos
g) Analog library Vdd, Gnd, Vcc, Vpulse, Vsin
h) Make the connections by using fixed narrow wire key i) Click Check and Save button
```
# Creating the Symbol for schematic Cell view
```
a. In the schematic window, execute Crate – Cell view – From Cell view The cell view from cell view window appears Check Lib Name, Cell Name, From View name must be schematic Press ok
b. Now Symbol generation form appears. Click Ok If No changes required
c. A new window with with default symbol is created.
d. Edit the symbol if you want to give actual symbol shape else continue. i. Execute Create-Cell view-from cell view ii. Library Name and Cell Name must be same which you have used for schematic. Press OK iii. Check for the position of pin side.Prss OK iv. Edit for the shape by Create-Shape-Choose required options to edit.
```
# Creating the new test cell view
```
a) Go to CIW window, Execute File-New-Cell view 
b) Setup the new file form Library: Select the one you a created. Cell: Cell name must be different from the name used in schematic cell view. Ex: Inverter_test View: Schematic Type: Schematic press OK
```
# Analog simulation by SPECTRE.
```
a. In test cell view window i. Launch – ADE L(Analog Design Environment)
b. Execute Setup—Simulation/directory/Host A new window opens
c. Set the simulation window to spectre and click ok
d. Execute Setup-Model Library. Anew window opens, Check of gpdk.scs as lib and section type as stat then press OK.
e. Execute Analysis – Choose. A window opens.
f. Select the type and set the specifications and press OK
g. Execute Output s—to be plotted – Select on Schematic
h. Then Select the INPUT WIRE(Vin ) and OUTPUT WIRE(Vout) from your test Schematic using mouse i. Execute Simulation -- Net list and Run
```
# INVERTER SCHEMATIC:
![WhatsApp Image 2024-05-20 at 13 12 52_cb355c1c](https://github.com/Afsar1276/VLSI-LAB-EXP-6/assets/161407741/f8e6ba72-4e13-4f0b-96a5-0d4ed148d688)

![WhatsApp Image 2024-05-20 at 13 13 17_5c36328b](https://github.com/Afsar1276/VLSI-LAB-EXP-6/assets/161407741/b8725ecd-9871-494f-828a-007eb00eb3a8)


# Specifications: Vpulse
```
V1 = 0
V2 = 1
td = 0,tr=tf=1 n, ton= 100n ,T=200n
Vdc = 1 Simulation Settings
Setup for transient analysis:
Stop time =400n
Setup for D.C analysis
Component to be selected in schematic is for d.c analysis
Start = -1 Stop = 1 resp. Expected Waveform:
```
# Transient Analysis:
![WhatsApp Image 2024-05-20 at 13 15 03_05f428b8](https://github.com/Afsar1276/VLSI-LAB-EXP-6/assets/161407741/69989bf2-73cf-4c74-8b91-a8697e0d8f21)

# DC Analysis:
![WhatsApp Image 2024-05-20 at 13 15 12_61a2296f](https://github.com/Afsar1276/VLSI-LAB-EXP-6/assets/161407741/bf6ef411-26db-4562-a5b4-43c7f75973e0)

# NAND SCHEMATIC :

![WhatsApp Image 2024-05-20 at 13 15 16_b2446a01](https://github.com/Afsar1276/VLSI-LAB-EXP-6/assets/161407741/f830e484-d7d3-45e2-af99-0fdceb81b174)

![WhatsApp Image 2024-05-20 at 13 15 28_77eec6ea](https://github.com/Afsar1276/VLSI-LAB-EXP-6/assets/161407741/1545d388-ada7-4aa0-852b-8fc97b051cbb)

# Specifications:
```
Vpulse
Va1 = 0 Va2 = 1 tr=tf=50ps, period=20ns pulse width = 10ns
Vb1 = 0 Vb2 = 1 tr=tf=50ps, period=40ns pulse width = 20ns
Vdc = 1
Expected Waveform:
```
# Transient Analysis:

![WhatsApp Image 2024-05-20 at 13 15 36_0e6d4594](https://github.com/Afsar1276/VLSI-LAB-EXP-6/assets/161407741/62e89507-a2d7-439b-99b7-1ad857463e17)

# NOR SCHEMATIC:

![WhatsApp Image 2024-05-20 at 13 15 51_5b907633](https://github.com/Afsar1276/VLSI-LAB-EXP-6/assets/161407741/897e3dcc-9135-422a-945e-3d61389286d1)

![WhatsApp Image 2024-05-20 at 13 15 56_84cfa5d6](https://github.com/Afsar1276/VLSI-LAB-EXP-6/assets/161407741/1c6aa4fb-a739-4965-9a7e-05677e187512)

# Specifications:
```
Vpulse
Va1 = 0 Va2 = 1 tr=tf=50ps, period=20ns pulse width = 10ns
Vb1 = 0 Vb2 = 1 tr=tf=50ps, period=40ns pulse width = 20ns
Vdc = 1
Expected Waveform:
```
# Transient Analysis: 

![WhatsApp Image 2024-05-20 at 13 16 02_4fa72453](https://github.com/Afsar1276/VLSI-LAB-EXP-6/assets/161407741/c03cfc51-c5bc-4852-af95-68554e18e3d0)

# RESULT:
Thus, the design,simulation and verification of the CMOS inverter,NAND,NOR from schematic using cadence was successfully completed.
