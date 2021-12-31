This folder contains various Python modules required for automation for DNA cloning.


### Run Sequence 

`IDT_Ordering_Module`
- Takes the designed oligos files, removes duplicates and created IDT ordering format. <br>

`Module 1`
- Re-format IDT files  

`Module 2`
- Add water to primers/guides, create picklists for Fluent.
- Create picklist for transfer to 384well plate for PCR setup.

`Module 3`
- Picklist for guide mixing and phosphorylation.

`Module 4`
- Picklist for primer and template mixing in Echo.
- There is an extension module for module 4 meant to be used for extension PCR. 

`Module 5`
- Equimolar mixing of PCR fragments.

Each module is dependent on successful run of the previous module. 



**There are two quality controls scripts as follows:**


`Assembled_Plasmid_Fragment_Validation`
- This module checks for two quality control items. First, The fragment numbering is correct in all annotated plasmids. Second, the DNA sequence is correctly labeled between different fragments. This module Should be run before the primer/guide design script. 


`Primer_Guide_Validation`
- This scripts validates that all designed primers and guides are a part of the original plasmid sequence. This script should be run before the IDT ordering module. 