# IOT SOLUTION TO DETECTING MISSING COMPONENT IN MOSFET DRIVER CIRCUIT PCB BOARDS


## Objectives:
To avoid any process failure due to missing components in a MOSFET DRIVER CIRCUIT PCB


## Methododolgy:

1) DataSet Generation
• Clicking images of each component of the PCB
• Crop them(Only PCB portion in image)
• Store them in server as black and white (2D array)
images with each file name as the name of the
component itself.
2) Algorithm Building
• Making use of ‘TEMPLATE MATCHING ’ creating
a project specific algorithm.
• What is TEMPLATE MATCHING?
template matching is to find a smaller image or
template into a larger image. The openCV library of
python has implementation of template matching.
• Applying this library we are building an algorithm
3) Implementation
• Implementing the template matching algorithm to
our data set and observing the outputs
• Based on the observations creating an algorithm that
solves the problem statement



## DESIGN: (SIMULATION)

1)A MOBILE APP TO SEND PICTURE OF PCB TO CLOUD

2)CLOUD HAS A IMAGE PROCESSING CODE TO DETECT MISSING COMPONENTS WITH THEIR LOCATION 

3)CLOUD WILL SEND NOTIFICATION BACK TO USER THROUGH MOBILE APP 
	



## ALGORITHM
1)Take images of all components of the PCB and convert
each of the colored( 3 dimensional RGB) images into
black and white(2D array) images and store these images
as templates

2) Also store the location data of each template by
usingthe correct PCB board

3) Find each component in the PCB board using the
templates stored and the template matching algorithm.

4) If the component location found by the algorithm
deviate by a very large value(¿500 or 600 units) then
the component should be considered as missing

5) If the component location does not deviate or deviates
very less (¡500 units) from the true location then the
component will be considered to be present in the PCB
board.


# How to run the app?
## Run the backend code in your google colab and also download the templates folder into your Google drive and change the filepaths accordingly in the python code.
## Download the apk file in your phone and start using the app to check any MOSFET TL9250 DRIVER PCB
## NOTE: If the output of the app is undesired then you can create your own templates and update the templates foder and then use the app.



	

