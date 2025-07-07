# full-volume-MRI
Sample full volume magnetic resonance imaging (MRI) datasets (displacements and strains) of intact and torn ovine rotator cuff tendons readable in Paraview.

Two folders are available: 20231012 and 20231107, which correspond to the timestamp of the experiment. 

Each folder has displacement and strain datasets. The displacement datasets can be visualized both in the intact and torn mesh. The prefix indicates the method used to unwrap the phase of the MRI: Jon for a code developed by Professor Jon Estrada, and sunwrap for the MATLAB function publicly available.

Both normal and shear components of the Lagrangian strain are available in the torn mesh. The codification is as follows: first number = displacement (1 for 1 mm, 2 for 2 mm), second number = condition (1 for intact, 2 for torn). The normal strain file has the 1-1, 2-2, and 3-3 components of the strain. The shear strain file has the 1-2, 1-3, and 2-3 components of the strain. Then, if the filename is 20231107LagrangeNormal_12.xdmf, it means that it has the 3 components of the normal strain for the 1 mm stretch, at the torn condition. Maximum shear strains are also available.
