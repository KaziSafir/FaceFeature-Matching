# FaceFeature-Matching
Python script demonstrates face and eye detection using OpenCV's Haar Cascade classifiers.

# Part 1: Import Necessary Libraries:

NumPy for numerical operations.

cv2 for computer vision tasks.

matplotlib.pyplot for plotting images.

# Part 2: Load Images:

The script loads three grayscale images: Julia-Roberts.jpg, NelsonMandela.jpg, and world_conference.webp.

# Part 3: Display Original Images:

Each loaded image is displayed in grayscale using Matplotlib.

# Part 4: Face Detection Using Haar Cascades:

A Haar Cascade classifier (haarcascade_frontalface_default.xml) is loaded for face detection.

A function face(img) is defined to detect faces in a given image, drawing rectangles around detected faces.

Face detection is applied to the images of Julia Roberts and Nelson Mandela, and the results are displayed.

# Part 5: Multi-Face Detection:

A separate function multiface(img) is defined to detect multiple faces in an image, suitable for images with more than one person.

The function uses detectMultiScale with a scale factor of 1.2 and a minimum of 2 neighbors to adjust detection sensitivity.

The function is applied to the world_conference.webp image to detect multiple faces, and the result is displayed.

# Part 6: Eye Detection Using Haar Cascades:

Another Haar Cascade classifier (haarcascade_eye.xml) is loaded for eye detection.

A function eyes(img) is defined to detect eyes in a given image, drawing rectangles around detected eyes.

Eye detection is applied to the images of Julia Roberts, Nelson Mandela, and the group photo from the world conference.

# Part 7: Observations:

The script notes that not all faces may be detected in the group photo, especially if they are not facing forward.

It also mentions that eye detection may not work perfectly due to factors such as squinting or poor image quality.
