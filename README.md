# 3D Slicer Lung Mask Generator
<br>
This extension enables the easy and quick production of three frequently used masks from lung CT scans: A "Right Lung Mask", a "Left Lung Mask" and a "Trachea mask".
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
<li>Define multiple markers by using the predefined marker widgets from the UI:
Place tem somewhere on the right lung, on the left lung, one in the middle of the trachea. </li>
<li>Press "Apply". </li>
<li>Check the masks, place additional markers if neede, press "Apply" again.</li>
  
</ul>
<br>After some seconds you should have fairly exact right and left lung masks. 
Always check the boundaries. <br>
<br>
Overview video: https://www.youtube.com/watch?v=DZ4T_0nONvo

<br>
<br>
Details
<br>
<br>
The script uses Slicer´s excellent "Segment Editor".
Developed and tested with Slicer 4.11.20200930.
<br>
<br>
This extension is suited to prepare the masks for the CT Lung Analyzer (https://github.com/rbumm/SlicerCTLungAnalyzer) of the same author.   
<br>
<br>
(1) https://www.slicer.org/
<br>
<br>
Idea and realization:<br>
<br>
Rudolf Bumm, Department of Surgery, Kantonsspital Graubünden (KSGR), Chur, Switzerland. <br>
<br>
<br>
Conceptual changes: Andras Lasso (PERK)
<br>
<br>
The code presented here is distributed under the Apache license (https://www.apache.org/licenses/LICENSE-2.0).<br>
<br>

