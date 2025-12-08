# Beauty Predictor

A machine learning project that analyzes facial attractiveness using the Chicago Face dataset. This project demonstrates both traditional ML approaches and deep learning techniques for facial analysis.

> **Disclaimer**: This project is for educational purposes and demonstrates how machine learning models can reflect societal biases. Beauty is subjective, and these models should not be used for serious evaluation. For more insights on algorithmic bias, see [this article](https://www.pavithra.dev/entries/beauty).

## Overview

The project uses the Chicago Face dataset containing approximately **597 individuals** with facial images, proportions, and attractiveness scores. The goal is to predict facial attractiveness through different computational approaches.

## Models

### Machine Learning Model
- **File**: `ML model- face proportions.ipynb`
- **Approach**: Regression-based model using mathematical analysis of facial dimensions
- **Input**: 25 facial measurements and ratios
- **Output**: Attractiveness score based on geometric features

### Deep Learning Models

#### Version 2 (CDF Dataset v2)
- **File**: `DL model.ipynb`
- **Dataset**: Chicago Face dataset version 2
- **Architecture**: CNN with transfer learning from VGG face dataset
- **Input**: Facial images
- **Output**: Attractiveness predictions

#### Version 3 (CDF Dataset v3)
- **File**: `DL model (cdf v3.0).ipynb`
- **Dataset**: Updated Chicago Face dataset version 3
- **Architecture**: Enhanced CNN with improved transfer learning
- **Model**: `model-cdf-v3-us.h5` (available in `/model` folder)
- **Complete Solution**: [Kaggle Notebook](https://www.kaggle.com/code/agrimrai29/cdf-us-trained-refined) - Complete dataset, code, and trained model
- **Input**: Facial images
- **Output**: Refined attractiveness predictions

The deep learning models process uploaded images and return attractiveness scores, while the ML model uses precise facial measurements for analysis.

## Data Sources

- The **Chicago Face dataset** can be downloaded or used from:  
  [Chicago Face Database](https://www.kaggle.com/datasets/agrimrai29/cdf-face-dataset-3-0-zip)  
  *(Note: A request form must be submitted stating your purpose for data access. A download link will be provided via email.)*

- The **VGG face model** is available here:  
  [VGG Face Model Download](https://www.kaggle.com/datasets/vincentscheltjens/vgg-face-weightsh5)

## Dimensions Required for the ML Model

To input measurements for the ML model, ensure you follow the specifications below. All measurements must be taken in centimeters, converted to inches (divide by 2.54), and multiplied by a factor of 100:

| Feature                     | Description                                                                                                       |
|-----------------------------|-------------------------------------------------------------------------------------------------------------------|
| Nose Width                  | Distance between the outer edges of the nostrils at the widest point.                                           |
| Nose Length                 | Distance from the bridge of the forehead (at the visible upper eye edge) to the nose tip.                        |
| Face Length                 | Distance from the hairline to the base of the chin. *(Estimate if a double chin is present.)*                   |
| Avg Eye Height              | Average distance between the upper and lower edges of the visible eye (centered on the pupil) for both eyes.     |
| Avg Eye Width               | Average distance from the inner to outer corners of each eye.                                                   |
| Face Width (Cheeks)        | Distance between the outer edges of the cheeks at their most prominent points.                                   |
| Forehead                    | Distance from the center of the hairline to the center between the eyes. *(Tip: A temporary box can help.)*     |
| Asymmetry (Pupil-Top)      | Absolute value difference in distance from the pupil center to the hairline for both sides.                       |
| Pupil-Lip Length            | Distance from the pupil center to the top edge of the lips.                                                     |
| Asymmetry (Pupil-Lip)      | Absolute value difference in distance from the pupil center to the top edge of the lips for both sides.          |
| Midcheek-Chin Length       | Distance from mid-cheek to the bottom of the chin.                                                              |
| Cheeks Avg                  | Average distance from mid-cheek to the bottom of the chin for both sides.                                       |
| Midbrow-Hairline Length     | Distance from mid-brow to the hairline, located above the pupil in the middle of the eyebrow.                   |
| Heartshapeness              | Ratio of face width at cheeks to face width at mouth.                                                           |
| Nose Shape                  | Ratio of nose width to nose length.                                                                               |
| Lip Fullness                | Ratio of lip thickness to face length.                                                                           |
| Eye Shape                   | Ratio of eye height to eye width.                                                                                 |
| Upper Head Length           | Ratio of forehead to face length.                                                                                |
| Midface Length              | Ratio of the average distance from pupil to lip for both sides to face length.                                   |
| Chin Length                 | Ratio of the distance from the bottom of the lip to the chin to face length.                                     |
| Forehead Height             | Ratio of the average distance from mid-brow to hairline for both sides to face length.                          |
| Cheekbone Height            | Ratio of the average distance from mid-cheek to chin for both sides to face length.                              |
| Cheekbone Prominence        | Ratio of the difference between face width at cheek and mouth to face length.                                    |
| Face Roundness              | Ratio of face width at mouth to face length.                                                                     |
| fWHR                        | Facial width to height ratio.                                                                                   |

---

