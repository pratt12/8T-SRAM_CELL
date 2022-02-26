
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
![The-schematic-diagram-of-8T-SRAM-cell](https://user-images.githubusercontent.com/69366735/155393461-8fe70052-4a97-47a5-a378-e62cc267b580.png) <br/>
However there is also a 
## Implementataion
The circuit for 8T SRAM built using synopsys design library tools is as below:
![schematic](https://user-images.githubusercontent.com/69366735/155392346-b4ab37cb-1efe-4d27-987c-2699c2fb1ff8.png)

## Netlist
Hold state circuit is reducesd to the following and the same is testes using testbench and wave viewer.
![holdm](https://user-images.githubusercontent.com/69366735/155856296-29256613-a37d-4c8a-aefe-583ed7d2b33c.png)



## Acknowledgements 
[Kunal Ghosh](https://github.com/kunalg123), Co-founder of VLSI System Design (VSD) Corp. Pvt. Ltd. <br />
[Indian Institute of Technology(IIT), Hyderabad](https://iith.ac.in/) <br />
[Synopsys](https://www.synopsys.com/)

## Author
Prateek Sinha: B.Tech(2023) Electrical Engineering at Indian Institute of Technology(IIT), Jammu. <br />
Email Id: 2019uee0127@iitjammu.ac.in

## References



