# Alert_System_for_Screen_Distance
## Function 1: 
This Function Calculate the Focal Length(distance between lens to CMOS sensor), it is simple constant we can find by using
MEASURED_DISTACE, REAL_WIDTH(Actual width of object) and WIDTH_OF_OBJECT_IN_IMAGE
:param1 Measure_Distance(int): It is distance measured from object to the Camera while Capturing Reference image
:param2 Real_Width(int): It is Actual width of object, in real world (like My face width is = 14.3 centimeters)
:param3 Width_In_Image(int): It is object width in the frame /image in our case in the reference image(found by Face detector)
:retrun focal_length(Float):
## Function 2:
This Function simply Estimates the distance between object and camera using arguments(focal_length, Actual_object_width, Object_width_in_the_image)
:param1 focal_length(float): return by the focal_length_Finder function
:param2 Real_Width(int): It is Actual width of object, in real world (like My face width is = 5.7 Inches)
:param3 object_Width_Frame(int): width of object in the image(frame in our case, using Video feed)
:return Distance(float) : distance Estimated

## Function 3:
This function Detect the face
:param Takes image as argument.
:returns face_width in the pixels
