# 8T-SRAM_CELL
The design and implementation of the 8T-SRAM Cell done by me was a part of an amazing initive i.e. [Cloud-based Analog Design Hackathon](https://www.iith.ac.in/events/2022/02/15/Cloud-Based-Analog-IC-Design-Hackathon/)  jointly conducted by IIT Hyderabad, VSD and Synopsys.
The whole process took place on Synopsys tool and the design implementation was done on 28nm PDK (Process Design Kit) 

## Table of Contents 
[Introduction](#introduction) <br />
[Reference Circuit](#reference-circuit) <br />
[Implementation](#implementataion)<br />
[Netlist](#netlist)<br />
[Acknowledgements](#acknowledgements) <br />
[Author](#author)<br/>
[References](#references)

## Introduction 
SRAM memory has become the key area of technology scaling as memory block becomes the main area consumer in high performance system. As the technology is advancing, so is the need to have more storage memory and that too in a compact form.Therfore the need for smaller cmos technologies is vital but as important is the need to improve the hold, read and write margin of the SRAM cell. In this implementation a very optimized 28nm technology is used and the simulations shown are for the hold and read margin of the SRAM Cell.
<br />
## Reference Circuit
This is the standard 8T SRAM Circuit and the testing involved the design and same simulation of the circuit as shown here. This Structure is better than 4T and 6T SRAMs.<br/>
<img src="https://user-images.githubusercontent.com/69366735/155393461-8fe70052-4a97-47a5-a378-e62cc267b580.png" width="500" height="300"/> <br/>
However there are many implementations on 8T SRAM based on the position of transistors as well as introduction of Transmission gates for better data transmission or based on low power needs as well.
## Implementataion
The circuit for 8T SRAM built using synopsys design library tools is as below:
<img src="https://user-images.githubusercontent.com/69366735/155392346-b4ab37cb-1efe-4d27-987c-2699c2fb1ff8.png" width="500" height="300"/> <br/>

## Netlist
### Hold state representation
2 CMOS looped inverter comprise the hold state of SRAM cell. The representation here is the CMOS inverter's change of state from 0 to 1 and if we were to take the mirror image of CMOS inverter 2 about the line y=x and superimpose on the same graph we would get the accurate representation of metastable point between the two inverters.  
<img src="https://user-images.githubusercontent.com/69366735/155856296-29256613-a37d-4c8a-aefe-583ed7d2b33c.png" width="500" height="300"/> <br/>
#### Hold state graph. <br/>
<img src="https://user-images.githubusercontent.com/69366735/155859682-9b723022-fd74-4e8e-a822-4d7f899eb450.png" width="600" height="400"/>
<br/>

### Write state representation <br/>
As you can see that there are just 6 transistors during the write state and this is due to the fact that rwl=0 and so we are left with the following schematic of transistors to implement the writing functionality in SRAM Cell
<img src="https://user-images.githubusercontent.com/69366735/155857395-68a800d0-0e9f-4efa-bbd4-9dadb0af6e67.png" width="500" height="300"/>
#### Write State graph
As you can see that during the write state rwl=0 making the 2 transistors in off state and so we are left with 6 transistors to implement the writing functionality in SRAM Cell.<br/>
<img src="https://user-images.githubusercontent.com/69366735/155859685-c4ef2d3d-571f-404a-aa66-f5e1eb2ccaba.png" width="600" height="400"/>

### Read state representation <br/>
Read state was also implemeted using 6 transistors as just as in the write state 2 transistors went off, here during read stage wwl=0 and so other two transistors are turned off and hence we are able to implement the read functionality in a transistor.
<img src="https://user-images.githubusercontent.com/69366735/155857644-1e01d1dc-83c3-43c3-81d7-7f65158cb296.png" width="500" height="300"/>
<br/>






## Acknowledgements 
[Kunal Ghosh](https://github.com/kunalg123), Co-founder of VLSI System Design (VSD) Corp. Pvt. Ltd. <br />
[Indian Institute of Technology(IIT), Hyderabad](https://iith.ac.in/) <br />
[Synopsys](https://www.synopsys.com/)

## Author
Prateek Sinha: B.Tech(2023) Electrical Engineering at Indian Institute of Technology(IIT), Jammu. <br />
Email Id: 2019uee0127@iitjammu.ac.in

## References
 1) Riya Patelia, “Static noise margin of 6T and 8T SRAM Cell in 28nmCMOS,” ICACM 2019,
 2)  Zhiyu Liu and Volkan Kursun, “Characterization of a Novel Nine Transistor SRAM Cell,” IEEE Transactions on Very Large Scale Integration (VLSI) Systems,VOL. 16, No.4,    April 2008.
 3)   Jitendra Kumar Mishra, Prasanna Kumar Misra and Manish Goswami,“A Low Power 7T SRAM cell using Supply Feedback Technique at28nm CMOS Technology,” 2020 7th International Conference on Signal Processing and Integrated Networks (SPIN)

