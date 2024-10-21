# K-Means Image Compression

This project implements K-Means clustering to perform image compression. By reducing the number of colors in an image, we can significantly decrease its file size while maintaining a visually similar appearance.

## Table of Contents

- [Introduction](#introduction)
- [How It Works](#how-it-works)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [License](#license)

## Introduction

Image compression is a crucial technique in computer graphics and data storage. This project utilizes the K-Means clustering algorithm to compress images by grouping similar colors and representing them with fewer color values. The result is a compressed image that retains the overall visual quality while using fewer bits of information.

## How It Works

1. **Image Loading**: The original image is loaded and normalized to ensure pixel values are in the range [0, 1].
2. **K-Means Initialization**: Randomly selected pixels serve as initial centroids for the K-Means algorithm.
3. **Clustering**: Each pixel is assigned to the nearest centroid based on color similarity.
4. **Centroid Update**: New centroids are computed as the mean of all pixels assigned to each centroid.
5. **Image Reconstruction**: The original image is reconstructed using the assigned centroids, resulting in a compressed version.
