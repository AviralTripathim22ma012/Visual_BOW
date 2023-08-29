## Steps for implementation:
1. Load the CIFAR-10 dataset: Load the CIFAR-10 dataset 
2. Extract features using SIFT: Use SIFT (Scale-Invariant Feature 
Transform) to extract features from the images in the training set. 
3. Perform K-means clustering: Cluster the extracted features into 
visual words using K-means clustering. This will create a codebook 
that will be used to represent the features of each image in the 
training set.
4. Create a histogram of visual words: For each image in the training 
set, create a histogram of visual words by counting the frequency 
of each visual word in the codebook that appears in the image.
5. Train a classifier: Use the histogram of visual words as features 
and the corresponding class labels as targets to train a classifier.
6. Extract features from the query image: Use SIFT to extract 
features from the query image.
7. Create a histogram of visual words for the query image: Create a 
histogram of visual words for the query image using the codebook 
created in step 3.
8. Compute similarity: Compute the similarity between the 
histogram of visual words of the query image and the histograms 
of visual words of all images in the training set using a similarity 
measure like the cosine similarity.

## Why was ORB unable to detect the features?
One possible reason why ORB may be unable to detect features in 
CIFAR 10 is that CIFAR 10 is a dataset of 
 small, low-resolution images that contain many similar-looking 
objects. The low-resolution of the images makes it difficult for 
ORB to detect distinctive features 
Another reason why ORB may be less effective in detecting features :
 CIFAR 10 is that it is primarily designed for detecting and matching 
features in natural images, where features tend to be welldefined and have high contrast. 
 the images in CIFAR 10 are not natural images, and the objects in 
them may not have clear features that can be easily detected by 
ORB

## Why was SIFT was able to detect the features?
 SIFT is intended to be scale-invariant, which is crucial for finding 
features in the CIFAR-10 dataset that are present at various 
scales. 
 Strong against occlusion: SIFT is also resistant to occlusion, 
making it useful for spotting details in CIFAR-10 photos where 
objects may be partially hidden by other objects or background 
clutter. Even if only a fraction of the object is visible, SIFT can still 
identify characteristics.
 Strong discriminative power: SIFT features have a high degree of 
discrimination, making them stand out from other features in the 
image. 
 Efficient: SIFT is a fast and accurate image processing approach 
that is well suited for identifying features in huge datasets like 
CIFAR-10.
