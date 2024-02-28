# Working-on-images
Working_on_images
AIM :
The image should be converted to gray scale and HSV and display the H, S and V planes.

Software Required :
jupyter Notebook

Algorithm :
Step1:
Choose an image , the image should be a plant , Tree, flower or building.

Step 2:
Save the image and the filename should be username.jpg

Step 3:
Convert the image to gray scale and HSV

Step 4:
Display the H,S and V planes.

Program :
Developed By : pocireddy.p
Register Number : 212223240115
import cv2
import numpy as np
username = "pochi"
image = cv2.imread("pochi.jpg")
image = cv2.resize(image,(300,200))
gray = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
hsv = cv2.cvtColor(image, cv2.COLOR_BGR2HSV)
h, s, v = cv2.split(hsv)
cv2.imshow("Hue (H)", h)
cv2.imshow("Saturation (S)", s)
cv2.imshow("Value (V)", v)
cv2.imwrite(f"{username}_gray.jpg", gray)
cv2.imwrite(f"{username}_hsv.jpg", hsv)
cv2.waitKey(0)
cv2.destroyAllWindows()
Output :
![Screenshot 2024-02-28 223811](https://github.com/pochireddyp/Working-on-images/assets/150232043/179886ef-bf07-4e11-9172-ff73f6e70961)


Result :
Thus the image is converted to gray scale and HSV using python and displayed successfully.
