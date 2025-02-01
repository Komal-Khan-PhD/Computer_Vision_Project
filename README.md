# Computer Vision Projects with OpenCV

Welcome to my **Computer Vision Projects** repository! This collection showcases my work on various computer vision tasks using **OpenCV** and **Python**. From basic image processing to advanced video manipulation, this repository demonstrates my skills in handling real-world computer vision challenges.

---

## 📁 **Projects Overview**

### **Image Processing**
1. **Reading and Displaying Images**  
   - Load and display images using OpenCV.
2. **Converting Images to Grayscale**  
   - Transform images into grayscale for easier processing.
3. **Converting Images to Black and White**  
   - Apply thresholding to create binary (black and white) images.
4. **Writing Images**  
   - Save processed images to disk.
5. **Basic Image Manipulations**  
   - Resize, blur, edge detection, and cropping of images.
6. **Drawing Lines and Shapes**  
   - Draw lines, rectangles, circles, and text on images.
7. **Joining Two Images**  
   - Stack images horizontally or vertically.
8. **Changing Image Perspective**  
   - Straighten documents or adjust image perspective.
9. **Face Detection in Images**  
   - Detect faces using Haar cascades.

### **Video Processing**
10. **Reading and Displaying Videos**  
    - Load and play video files.
11. **Converting Videos to Grayscale or Black and White**  
    - Process video frames to grayscale or binary.
12. **Writing Videos**  
    - Save processed videos to disk.
13. **Capturing Webcam Feed**  
    - Access and display live webcam feed.
14. **Converting Webcam Feed to Grayscale or Black and White**  
    - Real-time grayscale and binary conversion of webcam feed.
15. **Saving HD Webcam Recordings**  
    - Record and save high-definition video from a webcam.
16. **Splitting Videos into Frames**  
    - Extract individual frames from a video.

### **Advanced Features**
17. **Detecting Specific Colors**  
    - Use HSV color space to detect and isolate specific colors.
18. **Camera Settings and Resolution**  
    - Adjust camera settings like brightness, width, and height.
19. **Image Coordinates and Color Detection**  
    - Retrieve pixel coordinates and RGB values from images.
20. **Face Detection in Images**  
    - Detect and highlight faces in images using Haar cascades.

---

## 🛠️ **Technologies Used**
- **Python**: Primary programming language.
- **OpenCV**: For image and video processing.
- **NumPy**: For numerical operations and array manipulations.
- **Haar Cascades**: For face detection.

---

## 🚀 **How to Use This Repository**
1. Clone the repository:
   ```bash
   git clone https://github.com/Komal-Khan-PhD/Computer_Vision_Projects.git

2. Navigate to the project folder:
   ```bash
   cd Computer_Vision_Projects
   ```
3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Run the Jupyter notebooks or Python scripts to explore the projects.

---

## 📂 **Project Structure**
```
computer-vision-projects/
├── Image Processing/                   # Jupyter notebooks for image processing
├── Video Processing/                   # Jupyter notebooks for video processing
├── Advanced Features/                # Jupyter notebooks for advanced functionalities
├── README.md                 # This file
└── requirements.txt          # List of dependencies
```

---

## 📄 **Code Examples**
### Reading and Displaying an Image
```python
import cv2

# Load an image
img = cv2.imread("images/sample.jpg")

# Display the image
cv2.imshow("Sample Image", img)
cv2.waitKey(0)
cv2.destroyAllWindows()
```

### Face Detection in an Image
```python
import cv2

# Load the Haar cascade for face detection
face_cascade = cv2.CascadeClassifier("haarcascade_frontalface_default.xml")

# Load an image
img = cv2.imread("images/sample.jpg")
gray = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)

# Detect faces
faces = face_cascade.detectMultiScale(gray, 1.1, 4)

# Draw rectangles around detected faces
for (x, y, w, h) in faces:
    cv2.rectangle(img, (x, y), (x+w, y+h), (255, 0, 0), 2)

# Display the result
cv2.imshow("Detected Faces", img)
cv2.waitKey(0)
cv2.destroyAllWindows()
```

---

## 📈 **Contributions**
Feel free to contribute to this repository by:
- Reporting issues or bugs.
- Suggesting new features or improvements.
- Submitting pull requests with enhancements.

---

## 📧 **Contact**
If you have any questions or would like to collaborate, feel free to reach out to me:  
📧 **Email**: [dr.komalkhan@outlook.com](mailto:dr.komalkhan@outlook.com)  
💼 **LinkedIn**: [Komal Khan](https://www.linkedin.com/in/komalkhan31)  
🐱 **GitHub**: [Komal-Khan-PhD](https://github.com/Komal-Khan-PhD)

---

## 🌟 **Show Your Support**
If you find this repository helpful, please give it a ⭐️ star ⭐️ on GitHub!

---

**Happy Coding!** 🚀  

