# 3D Slicer Lung Mask Generator
<br>
This extension enables the easy and quick production of two frequently used masks from lung CT scans: A "Right Lung Mask" and a "Left Lung Mask".
This procedure is realized (semiautomatically) with 3D Slicer (1). 
<br>
<br>
Usage: 
<br>
<br>
<ul>
<li>Start 3D Slicer (1) and load a lung CT volume.</li>
<li>Start the "Lung Mask Generator" extension (what you see here, in "Chest Imaging Platform").</li>
<li>Select the appropriate volume from the input drop down menu. </li>
<li>Define four simple markers by using the predefined marker widgets from the UI:
Place one somewhere on the right lung, one on the left lung, one in the middle of the upper trachea above the thoracic aperture, the last one in the area of the tracheal bifurcation, orientated to the left main bronchus. </li>
<li>Press "Apply". </li>
</ul>
<br>After 20 seconds you should have a fairly exact right and left lung mask segmentation. 
Always check the boundaries. <br>
<br>
Overview video: https://www.youtube.com/watch?v=DZ4T_0nONvo

<br>
<br>
Details
<br>
<br>
The script uses Slicer´s excellent "Segment Editor".
First step is a threshold segmentation, which is then trimmed by "Surface Cuts" around the markers and a vertical lung mask division. 
Right and left lung mask are isolated by calling the "Islands" function and a "Keep selected island", much the same way you would do it by hand. 
Final touches are done to both masks by automatically applying the "Smoothing" function with a kernel size of 5 (to close most vessel, infiltration and bronchus holes). Developed and tested with Slicer 4.11.20200930.
<br>
<br>
This extension is ideally suited to prepare the masks for the CT Lung Analyzer (https://github.com/rbumm/SlicerCTLungAnalyzer) of the same author.   
<br>
<br>
(1) https://www.slicer.org/
<br>
<br>
Idea and realization:<br>
<br>
Rudolf Bumm, Department of Surgery, Kantonsspital Graubünden (KSGR), Chur, Switzerland. <br>
<a href="mailto:rudolf.bumm@ksgr.ch">Email</a>  <br>
<br>
<br>
The code presented here is distributed under the Apache license (https://www.apache.org/licenses/LICENSE-2.0).<br>
<br>

