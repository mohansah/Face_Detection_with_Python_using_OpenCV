# Face Detection with Python using OpenCV
Face detection is a computer vision technology that helps to locate/visualize human faces in digital images. This technique is a specific use case of object detection technology that deals with detecting instances of semantic objects of a certain class (such as humans, buildings or cars) in digital images and videos.

### OpenCV
OpenCV stands for Open Source Computer Vision Library.

### OpenCV-Python
OpenCV-Python is the python API for OpenCV. OpenCV-Python is not only fast (since the background consists of code written in C/C++) but is also easy to code and deploy(due to the Python wrapper in foreground). This makes it a great choice to perform computationally intensive programs.

### Face Detection
Face detection is a technique that identifies or locates human faces in digital images. A typical example of face detection occurs when we take photographs through our smartphones, and it instantly detects faces in the picture.

Face detection is different from Face recognition. Face detection detects merely the presence of faces in an image while facial recognition involves identifying whose face it is.

Face detection is performed by using classifiers. A classifier is essentially an algorithm that decides whether a given image is positive(face) or negative(not a face). A classifier needs to be trained on thousands of images with and without faces. Fortunately, OpenCV already has two pre-trained face detection classifiers, which can readily be used in a program. The two classifiers are:

1. Haar Classifier and
2. Local Binary Pattern(LBP) classifier.

## Haar feature-based cascade classifiers
Haar-like features are digital image features used in object recognition. This classifier is widely used for tasks like face detection in computer vision industry.

Haar cascade classifier employs a machine learning approach for visual object detection which is capable of processing images extremely rapidly and achieving high detection rates. This can be attributed to three main reasons:

1. Haar classifier employs 'Integral Image' concept which allows the features used by the detector to be computed very quickly.
2. The learning algorithm is based on AdaBoost. It selects a small number of important features from a large set and gives highly efficient classifiers.
3. More complex classifiers are combined to form a 'cascade' which discard any non-face regions in an image, thereby spending more computation on promising object-like regions.

## Methodology Used for Face Detection
1. Creating a CascadeClassifier Object and pass Path to the xml file which contains the face features as parameter.
2. Read the image in gray scale.
3. Method to search for the face rectangle co-ordinates.
4. Drawing rectangular face box
