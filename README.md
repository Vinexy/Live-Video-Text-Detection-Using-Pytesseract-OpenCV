![ezgif com-video-to-gif (9)](https://user-images.githubusercontent.com/85889196/227754190-390a42ba-ee25-4898-9bfb-3efa354d7eec.gif)


# Live-Video-Text-Detection-Using-Pytesseract-OpenCV
 
Python-tesseract is an optical character recognition (OCR) tool for python. That is, it will 
recognize and “read” the text embedded in images. Python-tesseract is a wrapper for 
Google's Tesseract-OCR Engine.  Tesseract developed from OCRopus model in Python which 
was a fork of a LSMT in C++, called CLSTM.

Using the Pytesseract library in Python, we made an image processing of a live video getting via webcam

![image](https://user-images.githubusercontent.com/85889196/175645853-9816d5d2-1c0c-4b45-bb6c-92071a955cda.png)

![image](https://user-images.githubusercontent.com/85889196/175645903-03eb945a-ade2-4302-ae91-ec2f6fa2d9ec.png)

![image](https://user-images.githubusercontent.com/85889196/175645957-3922a436-78c4-48fb-ae9b-16508c92d201.png)

# TEXT DETECTION FROM LIVE VIDEO

- Import pytesseract, cv2.
- Create a variable to read the frame using cv2.VideoCapture() function and pass
the name of the frame as parameter.
- Check the variable, is it reading or not. If it not raise an error.
- Set a counter, equalize it to zero. By having while loop counter help us to read 20
frame at a time.
- Read the values coming from VideoCapture() funtion. Increase counter value.
- Create two variables to store the dimensions of characters using frame.shape().
- Make imaginary text around each character using
pytesseract.image_to_boxes(frame)
- To convert to string use pytesseract.image_to_string(frame) and store it in a
variable.
- Create a for loop which converts all the coordinates in the form of list for easy
access.
- Initialize four variables for x-coordinate, y- coordinate, width, height.
- Assign their respective values from the above created list.
- As the list elements are in the form of string, convert it to integer.
- Use cv2.rectangle() function to create boxes around the characters.
- Use cv2.putText() to add labels around the characters.
- Use imshow() function to display frame.
- Show the results. If “q” is pressed finish the while loop and terminate the
Videcapture() function.
- Close tabs.
