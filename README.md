# Image Search using Visual Bag of Words

![Image Search](https://img.shields.io/badge/Image%20Search-Visual%20Bag%20of%20Words-blue.svg)
![CIFAR-10](https://img.shields.io/badge/Dataset-CIFAR--10-orange.svg)
![SIFT](https://img.shields.io/badge/Feature%20Extraction-SIFT-yellow.svg)
![K-means](https://img.shields.io/badge/Clustering-K--means-green.svg)
![Classifier](https://img.shields.io/badge/Classifier-Training-blueviolet.svg)

Welcome to the Image Search using Visual Bag of Words project repository! This project implements an image search system using the Visual Bag of Words technique, which is a popular method for content-based image retrieval.

## Overview

The Visual Bag of Words approach involves representing images as histograms of visual words, which are derived from local image features. These histograms are then used to measure the similarity between images.

## Steps for Implementation

1. **Load the CIFAR-10 dataset**: Load the CIFAR-10 dataset containing a diverse collection of images across ten classes.
2. **Extract features using SIFT**: Utilize the Scale-Invariant Feature Transform (SIFT) to extract distinctive features from the images in the training set.
3. **Perform K-means clustering**: Cluster the extracted features into visual words using K-means clustering, resulting in a codebook.
4. **Create a histogram of visual words**: For each image in the training set, generate a histogram of visual words by counting the frequency of each visual word from the codebook present in the image.
5. **Train a classifier**: Employ the histograms of visual words as features and the corresponding class labels as targets to train a classifier.
6. **Extract features from the query image**: Use SIFT to extract features from the query image.
7. **Create a histogram of visual words for the query image**: Generate a histogram of visual words for the query image using the codebook created in step 3.
8. **Compute similarity**: Calculate the similarity between the histogram of visual words of the query image and the histograms of visual words of all images in the training set using a similarity measure like cosine similarity.

## Usage

Feel free to explore the implementation provided in this repository. The project includes scripts for each step of the image search process, along with detailed instructions within each file.

## Requirements

- Python 3.x
- OpenCV
- NumPy
- scikit-learn

## Contributing

Contributions to this project are welcome! If you have ideas for improvements or new features, feel free to open an issue or submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE).

---

If you find this project useful or interesting, consider giving it a ⭐️!

[![GitHub stars](https://img.shields.io/github/stars/AviralTripathim22ma012/Visual_BOW.svg?style=social&label=Star)](https://github.com/AviralTripathim22ma012/Visual_BOW)
