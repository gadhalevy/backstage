# backstage
Software for  amateur theater class.
This project is based on Interactive Face Recognition Demo and need to be run within the directory of /opt/intel/openvino/deployment_tools/open_model_zoo/demos/python_demos/face_recognition_demo/.
The basic command line parameters for this project are defined in https://docs.openvinotoolkit.org/latest/_demos_python_demos_face_recognition_demo_README.html, besides I added more opthinal arguments to the gallery group:

'-cf', '--change_face', help=" Name of the actor you want to be replaced with another one (old)."
'-sw', '--switch_with', help=" Name of the actor you want to replace other actor (new)."
'-pp', help="Path to the different poses of the new actor (new)."

The application was built on linux 18.0.4 virtual box, it can be played with a camera (-i=1) or a video file (-i path to the video file) as input.
A list of persons witch appeare in the gallery can be defined after the -cf parameter, these people will be replaced with the list of people  after the -sw parameter, the lists have to be the same length no brackets needed.
Each person in the -sw list has two photos looking right and looking left, in a directory which his path defined after the -pp parameter.
The application identify each person on the screen and if that person was in the -cf list, replaces it with the person in the -sw list the original and the replaced person are in the same ordinal place in both lists.
As the application finds the the original person on screen looks right/left, the replaced looks right/left as well.


