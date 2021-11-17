# Classify images of characters from the office! Jim, Pam, Kelly, Dwight, and Micheal Scott!

The images have been sourced from the web by webscraping. 

For data cleaning - I found images with a clear face view i.e, two eyes must be visible. Done using OpenCV. If more than two faces are there, I manually selected the image. Opencv will crop face images.

Faces with two eyes are recognized using harr cascade and cropped. This is followed by a quick manual data cleaning, then the Wavelet Transform, and I finally train the model
Wavelet Transform extracts eyes, nose and face features. The orignal images and the transformed images are vertically stacked.

Built a python flask server using PyCharm to create a lightweight web server. Base64 encoding is used to convert the image to string and send to backend from UI.
The front end is designed using CSS, JS, HTML. Drop zone is used to input image.

### This includes:

- Created Dataset Using Web Scraping
- Image Transformations
- Analysis
- Haar Cascade Classifier for Object(Face) Detection
- Wavelet Transforms for Feature Extraction
- Using GridSearchCV for hypertuning parameters
- Training and Testing model:
	1. Support Vector Classifier
	2. Random Forest Classifier
	3. Logistic Regression


# To run, execute server.py and open the HTML file on your browser
