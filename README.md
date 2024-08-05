The code commpiled in this repository are all aspects used to track liquid lithium movement in the LTX-Beta tokamak. 
Written during the summer of 2024 during my SULI internship.
Each file has a brief description of the purpose/function of the code included.

This readme is a focus on the key aspects included in the code to be aware of. There are also comments throughout the code to help people follow what was done.
Cv2 was the main package used for formating images in the code.
Matplot lib was the main package used for plotting/displaying images.

In the lithium tracking algorithm the code is... (things that should be changed per shot)

the folder title 
crop the code and location that cropping starts from
brightness factor for the gamma filter
wait time in between frames (will affect elapsed time calculation)
start time, fast camera delay, and shot camera delay
can't have more than X bright spots in an image or else it is removed from all calculations



Other apsects that shouldn't be changed...

pixel to meter ratio
recognize what the 'previous' brightspot is for future parameters
definition for brightest spot
normalization to a 0 to 1 scale and normalization equation
can't have more than X brightest spots in an image or else it is removed from all calculations
the y pixel value must be less than the previous y pixel value (because it flows up and not down in the videos)
velocity is the change in x-pixel over elapsed time from previous frame


The code also has additional features for confirming tracking of the lithium or desired object. This is done through projecting various images and combinations of the videos side-by-side with or without a red tracking dot.
