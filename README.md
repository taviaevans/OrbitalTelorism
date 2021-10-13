# OrbitalTelorism
Processing and analysis of Orbital Teloirsm from MRI- used within # Cortex paper. 
Please reference # when using this method. 


Download atlas folder and unzip.

The files use high computational power to accuratly register the nateive space to the MNI space. A mask upon the MNI space outling the eyeballs is then registaerd to native space using the output from the inital registration. 
The center of gravity is exported for each eyeball mask and the distance between these is calculated for a proxy for Orbital telorism. 

The furtherst x,y,z coordinates are exported, and the min, max voxel value. These are used, along with the telorism distance to identify individuals where the processing has possibly failed to be manually checked (+/- 2 SD of these metrics). 

For cognitive/variable analysis you need three files that correspond to your data: in list format in the file.

* .dets
which includes the determinants in your analysis 
* .outs
which includes the variables of analysis
* .mods
which includes the variables adjusted for in each model
[example of * .mods file]

Age
Age+Sex
Age+Sex+Height



#for VBM processing pipeline please see https://github.com/roshchupkin/FSfslVBM





