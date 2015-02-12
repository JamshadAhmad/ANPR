ANPR
====
----------


**Algorithm**:

There are seven primary algorithms that the software requires for identifying a license plate:

 1. **[Plate localization](http://upload.wikimedia.org/wikipedia/commons/1/1a/LPR_Process.JPG)** : responsible for finding and isolating the plate on the picture.
 2. **Plate orientation and sizing** : compensates for the skew of the plate and adjusts the dimensions to the required size.
 3. **Normalization** : adjusts the brightness and contrast of the image.
 4. **Character segmentation** : finds the individual characters on the
    plates.
 5. **Optical character recognition**.
 6. **Syntactical/Geometrical analysis** : check characters and positions
    against country-specific rules.
 7. **The averaging** of the recognised value over multiple fields/images to produce a more reliable or confident result. Especially since any
    single image may contain a reflected light flare, be partially
    obscured or other temporary effect.

**Note :** The complexity of each of these subsections of the program determines the accuracy of the system. During the third phase (normalization), some systems use edge detection (like [canny](http://en.wikipedia.org/wiki/Canny_edge_detector)) techniques to increase the picture difference between the letters and the plate backing. 


----------


**Tips to improve:**
1) A camera that makes use of active infrared imaging (with a normal colour filter over the lens and an infrared illuminator next to it) benefits greatly.

![Infrared Camera](http://s4.postimg.org/l8lz6eizh/infrared_cameras.jpg)

2) A [**Median Filter**](http://en.wikipedia.org/wiki/Median_filter) may also be used to reduce the visual noise on the image.

Before / After (median filter)
--------------
![Before / After](http://upload.wikimedia.org/wikipedia/commons/1/1d/Medianfilterp.png)

----------


**Dificulties:**
- Poor file resolution.
- Blurry images, particularly motion blur.
- Poor lighting and low contrast due to overexposure, reflection or shadows.
- An object obscuring (part of) the plate, quite often a tow bar, or dirt infront of the camera.
- A different font, popular for vanity plates (some countries do not allow such plates, eliminating the problem).
- Circumvention techniques (Round or mixed characters fonts,using a plate cover or a spray).
- Lack of coordination between countries or states. Two cars from different countries or states can have the same number but different design of the plate.


**Still having perfect situation, there could be misreading due to** 

- Number plate partly out of field of view 
- Fixings (inappropriately located,damaged or rusting) 
- Mud 
- Cracks 
- Illegal font (or handwritten)
- Illegal character spacing 
- Illegal background 
- Illegal plate layout 
- Different reads in visible and InfraRed images 
- Character appearance alterations (black tape, IR-absorbing tape, ink etc.)

> Customers experience only ***90%*** to *94%* success, even with new equipment under **perfect** conditions. Early systems were reportedly only *60%* to *80%* reliable.

Click here for [__Reference__](http://en.wikipedia.org/wiki/Automatic_number_plate_recognition#Accuracy_and_measurement_of_ANPR_system_performance)


----------

Report by
---------

> jamshad.ahmad@coeus-solutions.de


----------


