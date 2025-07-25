# 3D K-Nearest Neighbors Implementation

This project implements a K-Nearest Neighbors (KNN) classifier from scratch using Python, with a 3D visualization of the classification process.

## Overview

The code provides a simple implementation of the KNN algorithm with the following features:
- Custom KNN classifier implementation
- 3D visualization of data points and classification
- Euclidean distance calculation
- Interactive plotting using Matplotlib

## Dependencies

- NumPy
- Matplotlib
- Collections (Python standard library)

## Usage

The code includes:
1. A `KNearestNeighbor` class that implements:
   - `fit()`: Trains the classifier with labeled data points
   - `predict()`: Classifies new points based on their k-nearest neighbors

2. Visualization features:
   - 3D scatter plot of training points
   - Different colors for each class (red and blue)
   - Dotted lines showing distances to the new point
   - Star marker (*) for the new point being classified

## Example

```python
# Create and train the classifier
clf = KNearestNeighbor(k=3)
clf.fit(points)

# Predict a new point
new_point = [3, 3, 4]
result = clf.predict(new_point)
```

## Visualization

The visualization includes:
- Blue points for one class
- Red points for another class
- Dotted lines showing distances to all training points
- Dark theme with grid for better visibility
- The new point marked with a star (*) in the color of its predicted class

## Implementation Details

The classifier uses Euclidean distance to measure the similarity between points and implements the standard K-nearest neighbors voting mechanism using the most common class among the k nearest
