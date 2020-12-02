# 3D Slicer Lung Mask Generator

This extension enables the easy production of two frequently used masks from lung CT scans: "Right lung mask" and "Left lung mask".

Usage: 

Start 3D Slicer and load a lung CT volume.
Start the Lung Mask Generator extension (in Chest Imaging Platform).   
Select the appropriate volume from the input drop do wn menu. 
Define four markers by using the predefined marker widges: 
Place one on the right lung, one on the left lung, one on the upper trachea above the thoracic aperture, the last one in the area of the tracheal bifurcation orientated to the left main bronchus. 
Press "Apply". 
After some seconds, you should have a fairly exact right and left lung mask segmentation. 

This procedure takes about 5 minutes and is only a fraction f the time you would have to use for manual production of the masks within SLicer. 

Details

The algorith m
