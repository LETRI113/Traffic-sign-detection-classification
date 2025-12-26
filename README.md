# Digital_Image_Processing_Final
Final project for Digital Image Processing. Detect and classify traffic signs from video using OpenCV, color thresholding, and labels

## 📂 Project Structure  
## Input and Output

https://drive.google.com/drive/folders/1GXl_1ilTnlSCmLjNeeRJBklsoHMU3Mf1?usp=sharing

🎯 Objectives

Detect traffic signs from video sequences

Classify detected signs using template matching

Apply classical image processing techniques instead of deep learning

Understand the full pipeline of a traditional computer vision system

🧠 Methodology (Classical Computer Vision Pipeline)

The system follows a traditional Digital Image Processing workflow:

Video Input

Read video frames using OpenCV

Color Space Conversion

Convert frames from RGB/BGR to HSV

HSV color space improves robustness for color-based segmentation

Color Thresholding

Apply predefined HSV thresholds to segment traffic sign colors

Generate binary masks for candidate regions

Morphological Operations

Use erosion and dilation to remove noise and refine detected regions

Contour Detection

Detect contours from binary masks

Filter contours based on geometric properties (area, shape, size)

Region of Interest (ROI) Extraction

Crop detected sign regions from the original frame

Template Matching

Compare extracted ROIs with stored templates

Classify traffic signs based on similarity scores

Visualization

Draw bounding boxes and predicted labels on video frames

⚠️ Note:
This project does NOT use deep learning, CNNs, or any trained models.
All techniques are based on classical computer vision and image processing.

🗂️ Project Structure

Digital_Image_Processing_Final/
│
├── processing.ipynb        # Main notebook implementing the processing pipeline
├── sign_templates/         # Template images for traffic sign classification
├── Report.pdf              # Project report (methodology and results)
├── README.md               # Project documentation

🛠️ Technologies Used

Python
OpenCV
NumPy
Matplotlib
Jupyter Notebook

📊 Key Features

Video-based traffic sign detection

Robust color segmentation using HSV

Classical contour-based object detection

Template matching for sign classification

Fully interpretable, rule-based computer vision pipeline

🚫 Limitations

Sensitive to lighting conditions

Performance depends on predefined color thresholds

Limited scalability compared to deep learning approaches

Requires manually prepared templates

📚 Academic Context

This project was developed as a final assignment for the Digital Image Processing course and focuses on applying fundamental image processing concepts, including:

Color models

Image segmentation

Morphological processing

Shape analysis

Template matching

📌 Possible Improvements

Adaptive thresholding for varying illumination

Shape-based feature extraction (Hu moments, HOG)

Integration with machine learning classifiers

Comparison with deep learning–based approaches

👤 Author

Lê Trí
Final-year student – Digital Image Processing
Ho Chi Minh City University of Technology and Education