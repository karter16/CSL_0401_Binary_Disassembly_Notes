CSL '0401' Binary Disassembly Notes
======
## Welcome
Welcome to this project which seeks to progress the understanding of the CSL '0401' program binary.

## How to Contribute
To contribute to this project please use the "Issues" feature to report discoveries of new information and bugs (issues identified with existing information). If you have general questions or would like to discuss particular items in general please use the "Discussions" feature.

At present the Ghidra project file is available for download. Any additions / changes you make to it will need to be reported back as a "Discovery" using the Issues feature. In the future this project will possibly use the Ghidra server functionality to make the master project file available to multiple contributors at once, but for now let's keep things simple.

The most important thing to be aware of when inspecting the project file is that 3 binaries are loaded to it:

Full 211323000401PD31_TERRA.bin  
Master  
Slave  

The first item is a load of the entire binary. The second and third are the Master and Slave components of the binary split out. The Master and Slave items are the ones that should be used for disassembly and discovery.

## Wiki
This project makes use of the wiki feature.  
  
[Identified Functions](https://github.com/karter16/CSL_0401_Binary_Disassembly_Notes/wiki/Functions)  
[Identified Variables](https://github.com/karter16/CSL_0401_Binary_Disassembly_Notes/wiki/Global-Variables)
[Identified Variables](https://github.com/karter16/CSL_0401_Binary_Disassembly_Notes/wiki/Global-Variables)  
[Unidentified Parameters/Curves/Maps](https://github.com/karter16/CSL_0401_Binary_Disassembly_Notes/wiki/Unidentified-Maps,-Curves-&-Parameters)  

## Disassembly Tools
This project uses [Ghidra](https://ghidra-sre.org) which is a very powerful open source Software Reverse Engineering (SRE) toolset developed by the NSA.
  
This project also relies on the [following files](https://github.com/NationalSecurityAgency/ghidra/commit/fafd1bb00aaca30ee546de0485896ba4de1bacab) which have been enhanced to add the appropriate CPU32 support (particularly the TBL lookup instructions).

Once Ghidra has been installed and the CPU32 support added the [project files](https://github.com/karter16/CSL_0401_Binary_Disassembly_Notes/blob/master/CSL_0401_Binary_Disassembly_2024_12_16.gar) can be opened.

## Reference Documents  
Below are details of the reference documents provided:

[CPU32RM.pdf](https://github.com/karter16/CSL_0401_Binary_Disassembly_Notes/blob/master/CPU32RM.pdf): This is the reference document for the CPU32 architecture that the MSS54HP processors are based on. Useful for referencing instructions, etc.
  
[MC68376.pdf](https://github.com/karter16/CSL_0401_Binary_Disassembly_Notes/blob/master/MC68376.pdf): This is the Motorola reference document for the MC68336/376 processors. As far as I can tell the MSS54HP uses the MC68336 or a very similar variant of it.
  
[Full 211323000401PD31_TERRA.bin](https://github.com/karter16/CSL_0401_Binary_Disassembly_Notes/blob/master/Full%20211323000401PD31_TERRA.bin): The full 0401 binary (with Terra's bootloader modifications) copied here for reference/posterity.
  
[MSS54 Funktionsrahmen (Original German)](https://github.com/karter16/CSL_0401_Binary_Disassembly_Notes/tree/master/MSS54%20Funktionsrahmen/Original%20(German)): The MSS54 funktionsrahmen documents for reference.  
[MSS54 Funktionsrahmen (Translated English)](https://github.com/karter16/CSL_0401_Binary_Disassembly_Notes/tree/master/MSS54%20Funktionsrahmen/Translated%20(English)): The MSS54 funktionsrahmen documents translated to English for reference.
