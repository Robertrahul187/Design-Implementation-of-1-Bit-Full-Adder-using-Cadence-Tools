# Design-Implementation-of-1-Bit-Full-Adder-using-Cadence-Tools
Ex No: 5     Design & Implementation of 1 Bit Full Adder Using Cadence EDA Tools   

Aim:
To design and implement a 1-bit full adder circuit using Cadence EDA tools and to understand its behavior in digital arithmetic operations.

Tools Required:
•	Personal Computer
•	Cadence Virtuoso Software

Circuit Diagram:

![WhatsApp Image 2024-11-13 at 4 26 07 PM](https://github.com/user-attachments/assets/115aa4ab-e285-41a6-879d-5b308a627990)


S C H E M A T I C S I M U L A T I O N - PROCEDURE FOR CREATING THE SCHEMATIC SIMULATION -Commands to get into Cadence

1.	Right Click and open the terminal window
2.	Type the following commands as follows and press enter.
•	csh
•	source /cadence/install/cshrc
•	virtuoso 
Procedure for Schematic simulation using Cadence

1.	Now two windows must open i) virtuoso/command interpreter window ii)”Whats New…”
2.	Close the 2nd window
3.	Use 1st window i.e virtuoso window (CIW) for further processing.
i.	Create a New Library
ii.	Create Schematic Cell view.
iii.	Create the Symbol for schematic Cell view.
iv.	Create the test Cell view.
v.	Analog simulation by spectre


i)	Procedure for Creating New Library.
•	File –New – Library
•	Name: Give name for ur library Ex: VLSILAB_EXP_1
•	Enable Attach to an existing technology library, Click OK
•	Attach the library to the technology library gpdk045.Click OK
ii)	Create Schematic Cell view.
•	Go to 1st window i.e virtuoso (CIW)
•	File-New-Cell view
•	Setup the new file form
	Library: Select the one you created.
	Cell: Give the experiment name Ex: Inverter ViewSchematic
	Type: Schematic press OK
•	Add the required components from the libraries and make the connections.
	Go to instance fixed menu or use shortcut key “I” from keypad to go instances
	Click on browse. This opens the library browser
	Now select the appropriate library for components like 
	Gpdk45 ------------------------nmos1v, pmos1v
	Create Input and Output pins
	Make the connections by using fixed narrow wire key
	Click Check and Save button

![EXP5(1)](https://github.com/user-attachments/assets/c6803d25-b0bf-43a8-9434-bab428df4e49)
![EXP5(2)](https://github.com/user-attachments/assets/bf60402c-c9ef-4b71-8e75-d8f982607476)
![EXP5(3)](https://github.com/user-attachments/assets/26b3882c-c894-43d9-8499-3c171893418c)
![EXP5(4)](https://github.com/user-attachments/assets/63ba0b16-9ac4-4553-8330-2a35e6cd5fa4)
![EXP5(6)](https://github.com/user-attachments/assets/f443fea8-850b-4c79-839a-8b378e14f9e6)


 
iii)	Creating the Symbol for schematic Cell view

•	In the schematic window, execute 
	Create – Cell view – From Cell view
	The cell view from cell view window appears
	Check Lib Name, Cell Name, From View name must be schematic Press ok
•	Now Symbol generation form appears. Click Ok If No changes required
•	A new window with with default symbol is created.
•	Edit the symbol if you want to give actual symbol shape else continue.
•	Execute Create-Cell view-from cell view
•	Library Name and Cell Name must be same which you have used for schematic. Press OK
•	Check for the position of pin side.Prss OK
•	Edit for the shape by Create-Shape-Choose required options to edit.

 ![IMG-20241019-WA0035](https://github.com/user-attachments/assets/dc5f18cf-8e4a-4970-a9bd-ced5c15fcfd9)



iv)	Creating the new test cell view

•	Go to CIW window, Execute File-New-Cell view
	Setup the new file form
	Library: Select the one you created.
	Cell: Cell name must be different from the name used in schematic cell view. Ex: Inverter_test
	View: Schematic
	Type: Schematic press OK
•	Follow the step 3(ii) d to make the required connections

![EXP5(5)](https://github.com/user-attachments/assets/ff011684-1336-4fe8-a76f-22dbd76db005)

 
Analog simulation by SPECTRE.
•	In test cell view window
•	Launch – ADE L(Analog Design Environment)
	Execute Setup—Simulation/directory/Host A new window opens
	Set the simulation window to spectre and click ok
	Execute Analysis – Choose. A window opens.
	Select the type and set the specifications and press OK
	Execute Output s—to be plotted – Select on Schematic
	Then Select the INPUT WIRE(Vin ) and OUTPUT WIRE(Vout) from your test Schematic using mouse
•	Execute Simulation -- Net list and Run
![EXP5(7)](https://github.com/user-attachments/assets/c6bf6f63-b1f6-428f-8060-bdaf1cc71473)


For Transient Analysis Settings and Output
 
![EXP5(8)](https://github.com/user-attachments/assets/4bac6287-ad93-4dbc-bf1b-119813c886fa)
![EXP5(9)](https://github.com/user-attachments/assets/9c221421-0160-4b8e-8ec1-c3dc54cb975f)


 

Results:
The design and implementation of the 1-bit full adder using Cadence EDA tools were successfully completed. The simulation results verified the correct operation of the full adder, with accurate sum and carry outputs for all input combinations.
