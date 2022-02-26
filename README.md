#  Schmitt Trigger NAND Gate 
This repository presents the design of Schmitt Trigger NAND gate implemented using Synopsis Custom Compiler on 28nm CMOS Technology.
# Table of Contents
- [Abstract](https://github.com/shivbaba/kirti/edit/main/README.md#abstract)
- [INTRODUCTION](https://github.com/shivbaba/kirti/edit/main/README.md#introduction)
- [Detailed Explanation](https://github.com/shivbaba/kirti/edit/main/README.md#detailed-explanation)
- [Tools Used](https://github.com/shivbaba/kirti/edit/main/README.md#tools-used)
- [Circuits and Waveforms](https://github.com/shivbaba/kirti/edit/main/README.md#circuits-and-waveforms)
- [CMOS NAND Gate](https://github.com/shivbaba/kirti/edit/main/README.md#cmos-nand-gate)
- [Symbol of CMOS NAND Gate](https://github.com/shivbaba/kirti/edit/main/README.md#symbol-of-cmos-nand-gate)
- [CMOS NAND Gate Waveform](https://github.com/shivbaba/kirti/edit/main/README.md#cmos-nand-gate-waveform)
- [Schmitt Trigger NAND Gate](https://github.com/shivbaba/kirti/edit/main/README.md#schmitt-trigger-nand-gate-1)
- [Symbol of Schmitt Trigger NAND Gate](https://github.com/shivbaba/kirti/edit/main/README.md#symbol-of-schmitt-trigger-nand-gate)
- [Schmitt Trigger NAND Gate Waveform](https://github.com/shivbaba/kirti/edit/main/README.md#schmitt-trigger-nand-gate-waveform)
- [Acknowledgements](https://github.com/shivbaba/kirti/edit/main/README.md#acknowledgements)

# Abstract
A two input Basic CMOS NAND gate can be implemented as a Schmitt trigger NAND gate by
adding one PMOS and NMOS at each p-stage and N-stage of the circuit.These transistors control the hysteresis width.By expanding the Schmitt trigger to NAND gate, we can dramatically improve the noise immunity with much lower switching power consumption and significant area reduction compared with CMOS Schmitt triggers, at the expense of a slight increase in delay.
# INTRODUCTION
NAND gate is important because we can implement any
type of boolean function using combination of NAND gate
and this property is known as functional completeness. The
function NAND (a1,a2,a3,……….an) is logically equivalent to
NOT (a1 AND a2 AND a3……AND an). 

For NAND gate, when both inputs are low, all PMOS transistors turn ON and the VDD is pulled to output as
high. When either of the inputs is high, VDD is pulled to Output as high through any current path formed by
PMOS devices. When both inputs are low, all PMOS transistors turn OFF, all NMOS transistors turn ON and
the output is low.
# Detailed Explanation
It consists of two series NMOS transistors between Z and
ground and two parallel PMOS transistor between Z and
VDD.

Case 1.: VA – Low: pMOS1 – ON; nMOS1 – OFF
 
 VB – High: pMOS2 – OFF; nMOS2 – ON

Case 2 : VA – High: pMOS1 – OFF; nMOS1 – ON
 
 VB – Low: pMOS2 – ON; nMOS2 – OFF

Case3: VA – High: pMOS1 – OFF; nMOS1 – ON
 
 VB – High: pMOS2 – OFF; nMOS2 – ON

Case4: VA – Low & VB – Low

Both the pMOS will be ON and both the nMOS will be OFF

# Circuits and Waveforms
# CMOS NAND Gate

![101](https://github.com/shivbaba/kirti/blob/main/cmos%20nand.png)
                    NAND GATE SCHEMATIC

# Symbol of CMOS NAND Gate
![102](https://github.com/shivbaba/kirti/blob/main/nand%20symbol.png)

# CMOS NAND Gate Waveform

![103](https://github.com/shivbaba/kirti/blob/main/cmos%20nand%20waveform.png)
                    SIMULATION RESULT 

# Schmitt Trigger NAND Gate
![104](https://github.com/shivbaba/kirti/blob/main/schmit%20triiger%20nand%20schematic.png)

Schmitt Trigger NAND GATE SCHEMATIC
  
# Symbol of Schmitt Trigger NAND Gate
![105](https://github.com/shivbaba/kirti/blob/main/schmitt%20trigger%20nand%20symbol.png)

# Schmitt Trigger NAND Gate Waveform
![106](https://github.com/shivbaba/kirti/blob/main/schmitt%20nand%20waveform.png)
SIMULATION RESULT 




# Tools Used
•	Synopsys Custom Compiler:  The Synopsys Custom Compiler™ design environment is a modern solution for full-custom analog, custom digital, and mixed-signal IC design. As the heart of the Synopsys Custom Design Platform, Custom Compiler provides design entry, simulation management and analysis, and custom layout editing features. This tool was used to design the circuit on a transistor level.

•	Synopsys Primewave:  PrimeWave™ Design Environment is a comprehensive and flexible environment for simulation setup and analysis of analog, RF, mixed-signal design, custom-digital and memory designs within the Synopsys Custom Design Platform. This tool helped in various types of simulations of the above designed circuit.

•	Synopsys 28nm PDK:  The Synopsys 28nm Process Design Kit(PDK) was used in creation and simulation of the above designed circuit.

# Acknowledgements
- [Kunal Ghosh, Co-founder, VSD Corp. Pvt. Ltd.](https://www.iith.ac.in/events/2022/02/15/Cloud-Based-Analog-IC-Design-Hackathon/)
- [Cloud Based Analog IC Design Hackathon](https://www.iith.ac.in/events/2022/02/15/Cloud-Based-Analog-IC-Design-Hackathon/')
- [Synopsys India](https://www.synopsys.com/)
- [Sameer Durgoji, NIT Karnataka](https://www.iith.ac.in/events/2022/02/15/Cloud-Based-Analog-IC-Design-Hackathon/)
- [Chinmay panda, IIT Hyderabad](https://www.iith.ac.in/events/2022/02/15/Cloud-Based-Analog-IC-Design-Hackathon/)
