# ENCM 509 Final Project

## Description
This project focuses on developing and comparing various facial detection systems using a human face database to determine which method achieves the highest accuracy in identifying faces with minimal detection errors. Through this comparative analysis, we aim to establish the most effective approach to facial detection, which serves as a fundamental component for advanced applications like facial recognition systems.

## Instructions

1. Clone the repository
```bash
git clone [repository-url]
```

2. Run the Jupyter Notebook
   - Open `face_detection.ipynb`
   - Run all cells sequentially

   **Note regarding dlib installation:**
   If you encounter issues with dlib installation, modify the installation command in the notebook:
   ```python
   # Option 1 (default):
   !pip install dlib

   # Option 2 (if Option 1 fails):
   # !pip install "dlib-19.22.99-cp38-cp38-win_amd64.whl"
   ```

## Data Structure
- The actual image files are stored in `data/images`
- The source truth bounding boxes for each images are in `data/labels`
- The coordinates for the bounding boxes are located in `corrected.xml`
- `face_detection.csv` maps the image filepath to the label filepath

## Code Structure
- The required packages are first installed
- Load Data - reads in the image and bounding box data
- Helper Functions - functions used to display images and calculating metrics
- The 3 algorithms (metrics calculated for each within its respective sections)
    - Original Haar Cascades
    - LBP-based Haar Cascades
    - HOG + SVM

## Contributors
- Sukriti Sharma
- Caroline Basta