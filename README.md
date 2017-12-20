# OCR-App
A basic OCR application 

This is a basic OCR application which can recognize a single character. It is based on the principle of machine learning
which involves teaching(or training) the program with a given dataset and allowing the program to act on a new dataset
(or testing).

Objectives: To predict which family the given dataset belongs to with feasible accuracy(x or not x)

Input: Using the OpenCV module, which is used for image processing, 120 images are formatted and stored as n-dimensional
       arrays(trainData). Each image is assigned a label which is stored in another array(trainLabel). The test data can 
       either be a single image or an array of images.
		 	
Processing : Using numpy and OpenCV, images are processed and stored as arrays of 20x20 pixel images. This program is
             based on the k Nearest Neighbours(kNN) algorithm which takes a given dataset and 'learns' from it. Once this
             has been done, a new dataset may be classified into a group based on the given dataset(in this case, x's
             handwriting or not x's handwriting).

Output: Depending on usage the program either returns:
	i) A sentence saying if the given image was of x's handwriting or not.  
	ii) A percentage value denoting the number of correct assignments had done in an array of input images.

Limitaions: i) Depending on the value of k the accuracy of the program will change.
	    ii) Too many outliers will reduce the usefulness of this program.
	    iii) It is very easily affected by noise(unimportant data).
	    iv) If thei images are not formatted properly the program's effectiveness will be lowered a lot.
	    v) As with all machine learning programs, the number of training samples given increases accuracy thus 
	       requiring  a large number of samples to be feasible.	
	    vi) Computationally expensive.	
