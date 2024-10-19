# Beauty-Predictor

> ⚠️ **Disclaimer**: This beauty predictor model is purely a hobby project, created for the sole purpose of showcasing how machine learning can be influenced by biases—because, let’s be honest, even algorithms can fall victim to society’s quirks! Remember, beauty is subjective, and if your score isn’t what you hoped, just blame it on the dataset! For a deeper dive into these biases (and a few laughs), check out my article [here]([#](https://pavithra.dev/entries/beauty)). 

This project utilizes the **Chicago Face dataset** to develop both a **Machine Learning (ML)** model and a **Deep Learning** model with **Convolutional Neural Networks (CNN)** and transfer learning from the **VGG face dataset**. 

## Overview

The Chicago Face dataset comprises images of approximately **597 individuals**, encompassing both males and females, along with facial proportions and attractiveness scores. The primary aim of this model is to assess facial attractiveness based on various facial dimensions.

### Models

1. **Machine Learning Model**: 
   - This regression-based model evaluates facial attractiveness through mathematical assessments of facial dimensions.
  
2. **Deep Learning Model**: 
   - Utilizing transfer learning with the VGG face dataset, this model processes images of the 597 individuals to predict attractiveness scores purely based on image data.

Users can upload an image to the Deep Learning model, which will return an attractiveness score based on the visual data, while the ML model applies a more mathematical approach.

## Data Sources

- The **Chicago Face dataset** can be downloaded from:  
  [Chicago Face Database](https://chicagofaces.org/default/)  
  *(Note: A request form must be submitted stating your purpose for data access. A download link will be provided via email.)*

- The **VGG face model** is available here:  
  [VGG Face Model Download](https://drive.google.com/file/d/1CPSeum3HpopfomUEK1gybeuIVoeJT_Eo/view?usp=sharing)

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

