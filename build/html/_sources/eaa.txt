.. _eaa:

EAA Stacker
===========

EAA stacker will assist you to easily stack images and make a great visualization of deep sky object with your existing telescope.

What is Image Stacking?
-----------------------

The raw images from an image sensor is usully quite noisy. One of the simplest way to handle such noise is to take multiple images and getting an averaged image. EAA stacker support multiple useful tools for image stacking. 

Exposure Time and Gain
------------------------
Exposrue time and gain can be adjusted according to your pefernce. Short exposure time enable the EAA stacker to be more responsive to the mount movement and creates less blurly image when used with longer focal lenght lens. Long exposure can reduce image noise but it can cause unwanted star trails especially on manual and Altazimuth mounts.

Adjusting the gain to a higher value will amplify some faint signal such as nebular and make it more visible while it increase noises on the image. 160 or lower is recommanded for the gain. When there is too much noise due to the high gain value, increasing the stacking image number will lower the overall noise level.  


Installation Example
---------------------

50.8mm

Eyepiece

Direct lens connection

Stack Mode
------------
EAA Stacker supports two stack modes: with and without tracking. Tracking mode automatically align input images to the first image that was captured when the live stack mode was turned on. This is especially useful on a manual mount and Altazimuth mount as the outcome looks a static view. Turning off the tracking mode will be required when the lens is dark and EAA stacker does not find a star to track. For example, any lens above F5 might cause frequent tracking reset due to lack of trackable stars in the image. You can adjust gain to make the stars are visible enough for tracking. You can also turn off the tracking mode will let EAA stacker simpley average images without alignment. Note that when tracking option is off you must turn on the phical tracking option on your mount.

Mean Substraction
------------------

If the stacked image is too bright check this option. This option estimates the mean RGB value of the stacked image and subtract it. Use this option if you are using EAA stacker under the sky with light pollution.


Tone Curve
-----------




Stacking Number
----------------

The number of images to be stacked can be adjusted through this option. The stacking number 4, 8, 16 add all the image on the buffer and devide by each stacking number whereas 32, 64 add without division for a darker lens. 


