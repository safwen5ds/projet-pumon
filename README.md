#Medical CT Scan Analysis for Lung Tumor Detection

**Author:** Gharbi Safwen CI 1

## Description

This project implements medical image analysis techniques for detecting lung tumors in CT scan images. The notebook demonstrates a complete pipeline for medical image processing, including lung segmentation and tumor identification using computer vision techniques.

## Features

- **Medical Image Processing**: Specialized techniques for CT scan analysis
- **Lung Segmentation**: Automatic isolation of lung regions from CT images
- **Tumor Detection**: Identification and highlighting of potential tumor areas
- **Multi-stage Visualization**: Step-by-step display of the analysis process
- **Morphological Operations**: Advanced image processing for noise reduction

## Installation

Install the required dependencies:

```bash
pip install opencv-python matplotlib numpy
```

For Google Colab users:
```bash
from google.colab.patches import cv2_imshow
```

## How It Works

### Image Processing Pipeline

1. **Image Loading**: Loads CT scan images (expects CT001.jpg format)
2. **Color Space Conversion**: Converts from BGR to RGB for proper display
3. **Grayscale Conversion**: Converts to grayscale for analysis
4. **Gaussian Blur**: Applies noise reduction using Gaussian filter
5. **Otsu Thresholding**: Automatic threshold selection for binarization
6. **Morphological Operations**: Dilation and erosion for shape refinement
7. **Contour Detection**: Identifies lung boundaries
8. **Lung Segmentation**: Isolates lung regions using mask
9. **Tumor Detection**: Identifies potential tumor areas
10. **Tumor Highlighting**: Colors detected tumors in yellow

### Key Processing Steps

- **Preprocessing**: Blur and threshold operations for noise reduction
- **Mask Creation**: Binary mask generation for lung isolation
- **Contour Analysis**: Detection of anatomical structures
- **Region Segmentation**: Separation of lung tissue from background
- **Tumor Identification**: Detection of abnormal tissue areas
- **Visualization**: Multi-panel display of analysis results

## Usage

1. Place your CT scan image named `CT001.jpg` in the appropriate directory
2. Run the notebook cells sequentially
3. The system will automatically:
   - Load and preprocess the CT image
   - Segment the lung regions
   - Detect potential tumor areas
   - Display comprehensive analysis results

## Output Visualization

The analysis produces a 4-panel visualization:

1. **Original Image**: Raw CT scan input
2. **Lung Mask**: Binary mask showing detected lung regions
3. **Segmented Lungs**: Isolated lung tissue only
4. **Tumor Detection**: Final result with tumors highlighted in yellow

## Medical Applications

This type of analysis is valuable for:
- **Diagnostic Imaging**: Assisting radiologists in tumor detection
- **Screening Programs**: Automated analysis of large image datasets
- **Treatment Planning**: Precise localization of abnormal tissue
- **Research**: Quantitative analysis of lung pathology
- **Quality Assurance**: Standardized image analysis protocols

## Technical Implementation

### Image Processing Techniques
- **Gaussian Filtering**: Noise reduction while preserving edges
- **Otsu Thresholding**: Automatic threshold selection
- **Morphological Operations**: Shape analysis and refinement
- **Contour Detection**: Boundary identification
- **Mask-based Segmentation**: Region isolation

### Visualization Features
- **Multi-panel Layout**: Comprehensive result display
- **Color Coding**: Yellow highlighting for tumor areas
- **Grayscale Processing**: Standard medical imaging format

## File Requirements

- Input CT scan image: `CT001.jpg`
- Image should be in standard CT scan format
- Recommended resolution: High-resolution medical imaging

## Important Notes

⚠️ **Medical Disclaimer**: This is an educational project for learning image processing techniques. It should not be used for actual medical diagnosis without proper validation and clinical oversight.

## Technical Details

- **Environment**: Designed for Google Colab
- **Image Format**: Supports standard medical imaging formats
- **Processing**: OpenCV-based computer vision pipeline
- **Visualization**: Matplotlib for medical image display

## Limitations

- Currently configured for specific image naming convention
- Requires manual adjustment of contour selection parameters
- Not validated for clinical use 
