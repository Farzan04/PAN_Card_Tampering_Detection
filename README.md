PAN Card Tampering Detection

A program for detecting tampering of PAN card using Computer Vision.
This project will help different organization in detecting whether the Id i.e. the PAN card provided to them by thier employees or customers or anyone is original or not.
**Steps:
* Create directory for downloading images uploaded by user.
* Convert the format and size of tampered image similar to original image.
* Read images using opencv.
* Convert images into grayscale using opencv: 
 --> Because in image processing many applications doesn't help us in identifying the important, edges of the coloured images also coloured images are bit complex to understand by machine beacuse they have 3 channel while grayscale has only 1 channel.
 * We will calculate Structural similarity:
 --> Structural similarity index helps us to determine exactly where in terms of x,y coordinates location, the image differences are. Here, we are trying to find similarities between the original and tampered image. The lower the SSIM score lower is the similarity.
* Calculate Threshold and Contours:
--> Threshold is a function of computer vision which applies an adaptive threshold to the image which is stored in the form array. This function transforms the grayscale image into a binary image using a mathematical formula
--> Contours are a useful tool for shape analysis and recoginition. Grab contours grabs the appropriate value of the contours.
* Display Bounding rectangles:
--> Bounding rectangle helps in finding the ratio of width to height of bounding rectangle of the object. We compute the bounding box of the contour and then draw the bounding box on both input images to represent where the two images are different or not.
  
  *** This python program can be used in different organizations where customers or users need to provide any kind of id in order to get themselves verified. The organization can use this project to find out whether the ID is original or fake. Similarly this can be used for any type of ID like adhar card, voter id, etc. ***
