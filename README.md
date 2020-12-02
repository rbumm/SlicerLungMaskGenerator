# 3D Slicer Lung Mask Generator
<b>
This extension enables the easy production of two frequently used 3D Slicer (1) masks from lung CT scans: "Right lung mask" and "Left lung mask".
<b>
Usage: 
<b>
Start 3D Slicer and load a lung CT volume.
Start the "Lung Mask Generator" extension (what you see here, hopefully in "Chest Imaging Platform" soon).   
Select the appropriate volume from the input drop do wn menu. 
Define four simple markers by using the predefined marker widgets fro the UI: 
Place one somewhere on the right lung, one on the left lung, one in the middle of the upper trachea above the thoracic aperture, the last one in the area of the tracheal bifurcation, orientated to the left main bronchus. 
Press "Apply". 
After some seconds, you should have a fairly exact right and left lung mask segmentation. 
Please check the boundaries and manually trim if you are not satisfied. 
<b>
Details
<b>
The script uses Slicer´s excellent "Segment Editor".
First step is a threshold segmentation, which is then trimmed by "Surface Cuts" around the markers and a vertical lung mask division. 
Right and left lung mask are isolated by calling the "Islands" function and a "Keep selected island", much the same way you would do it by hand within SLicer. 
Final touches are done to both masks by applying the "Smoothing" function with a kernel size of 5 (to close most vessel, infiltration and bronchus holes).  
<b>
(1) https://www.slicer.org/
<b>
Idea and realization:<b>
Prof. Rudolf Bumm<b>
Department of Surgery<b>
Kantonsspital Graubünden<b>
Chur, Switzerland<b>
<b>
(c) 2020 by R. Bumm, Munich / Chur.<b>
All rights reserved. <b>
The code presented here is distributed under the Apache license (https://www.apache.org/licenses/LICENSE-2.0).<b>
<b>
Development and marketing: c/o Scientific-Networks Munich<b>
info@scientific-networks.com<b>

