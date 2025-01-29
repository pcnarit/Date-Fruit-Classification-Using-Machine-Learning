# Date-Fruit-Classification-Using-Machine-Learning
A machine learning model to classify different varieties of date fruits based on external features such as color, length, diameter, and shape factors. The dataset is obtained from Murat Koklu's research on genetic classification using image analysis.

## Objective
To determine the variety of date fruit using data describing the **colour**, **length**, **diameter**, and **shape**.

## Data
The dataset is obtained from [DATASETS (muratkoklu.com)](http://muratkoklu.com) and was used in the following publication:

- **M. Koklu, R. Kursun, Y.S. Taspinar, and I. Cinar**, "Classification of Date Fruits into Genetic Varieties Using Image Analysis," *Mathematical Problems in Engineering*, Vol. 2021, Article ID: 4793293 (2021).

## Problem Statement
In food production, accurate labeling of ingredients is crucial for both health and business purposes. However, mistakes can happen, and there is significant room for improvement in food labeling practices.

A variety of dates are grown globally, and identifying the specific type requires expertise. The task is to build a machine learning model that can classify the type of date fruit based on external features such as:

- **Colour**
- **Length**
- **Diameter**
- **Shape factors**

These features have been extracted using a computer vision model.

## Task
As a machine learning developer, your goal is to develop a classification model capable of identifying the variety of date fruits from the given features.

---
## Explanation of the Columns and Dataset Observations

### **1. Morphological Features**
These features describe the physical shape and size of the date fruits:
- **AREA**: The total number of pixels representing the fruit's surface.
- **PERIMETER**: The boundary length of the fruit in pixels.
- **MAJOR_AXIS**: The longest diameter of the fruit's shape.
- **MINOR_AXIS**: The shortest diameter perpendicular to the major axis.
- **ECCENTRICITY**: A measure of how elongated the fruit is, ranging from 0 (circular) to 1 (elongated).
- **EQDIASQ** (Equivalent Diameter): The diameter of a circle with the same area as the fruit.
- **SOLIDITY**: The ratio of the fruit's area to its convex hull area, indicating how compact the shape is.
- **CONVEX_AREA**: The area of the smallest convex polygon enclosing the fruit.
- **EXTENT**: The ratio of the fruit’s area to the bounding box area, showing how much space the fruit occupies in its box.
- **ASPECT_RATIO**: The ratio of the major axis to the minor axis.
- **ROUNDNESS**: Measures how circular the shape is.
- **COMPACTNESS**: A measure of how closely packed the fruit's pixels are.

---

### **2. Shape Features**
These features quantify more intricate shape-related properties:
- **SHAPEFACTOR_1**: Relates to shape complexity based on area and perimeter.
- **SHAPEFACTOR_2**: Another measure of shape irregularity.
- **SHAPEFACTOR_3**: Combines compactness and roundness to describe shape.
- **SHAPEFACTOR_4**: Focuses on the curvature of the fruit's boundary.

---

### **3. Color Features**
These features describe the color distribution of the fruit:
- **MeanRR, MeanRG, MeanRB**: Average values of red, green, and blue intensities in the image.
- **StdDevRR, StdDevRG, StdDevRB**: Standard deviations of red, green, and blue intensities, indicating variability.
- **SkewRR, SkewRG, SkewRB**: Skewness of the red, green, and blue intensities, showing the asymmetry of color distribution.
- **KurtosisRR, KurtosisRG, KurtosisRB**: Kurtosis of red, green, and blue intensities, describing the "tailedness" of the color distribution.
- **EntropyRR, EntropyRG, EntropyRB**: Entropy measures the randomness in color intensity distributions.
- **ALLdaub4RR, ALLdaub4RG, ALLdaub4RB**: Daubechies 4 wavelet features of the red, green, and blue channels, used for texture analysis.

---

### **4. Class**
- The **Class** column identifies the type of date fruit ('BERHI', 'DEGLET', 'DOKOL', 'IRAQI', 'ROTANA', 'SAFAVI', 'SOGAY').

---
