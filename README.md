# 3D Slicer Lung Mask Generator
<br>
This extension enables the easy and quick production of two frequently used 3D Slicer masks from lung CT scans: "Right lung mask" and "Left lung mask".
<br>
<br>
Usage: 
<br>
Start 3D Slicer (1) and load a lung CT volume.
Start the "Lung Mask Generator" extension (what you see here, hopefully in "Chest Imaging Platform" soon).   
Select the appropriate volume from the input drop down menu. 
Define four simple markers by using the predefined marker widgets fro the UI: 
Place one somewhere on the right lung, one on the left lung, one in the middle of the upper trachea above the thoracic aperture, the last one in the area of the tracheal bifurcation, orientated to the left main bronchus. 
Press "Apply". 
After some seconds, you should have a fairly exact right and left lung mask segmentation. 
Please check the boundaries. 
<br>
<br>
Details
<br>
The script uses Slicer´s excellent "Segment Editor".
First step is a threshold segmentation, which is then trimmed by "Surface Cuts" around the markers and a vertical lung mask division. 
Right and left lung mask are isolated by calling the "Islands" function and a "Keep selected island", much the same way you would do it by hand. 
Final touches are done to both masks by applying the "Smoothing" function with a kernel size of 5 (to close most vessel, infiltration and bronchus holes). Development and testing with Slicer 4.11.20200930.
<br>
<br>
This extension is ideally suited to prepare the masks for the CT Lung Analyzer (https://github.com/rbumm/SlicerCTLungAnalyzer) of the same author.   
<br>

(1) https://www.slicer.org/
<br>
<br>
Idea and realization:<br>
Prof. Rudolf Bumm<br>
Department of Surgery<br>
Kantonsspital Graubünden<br>
Chur, Switzerland<br>
<br>
<br>
(c) 2020 by R. Bumm, Munich / Chur.<br>
All rights reserved. <br>
The code presented here is distributed under the Apache license (https://www.apache.org/licenses/LICENSE-2.0).<br>
<br>
Development and marketing: c/o Scientific-Networks Munich<br>
info@scientific-networks.com<br>

