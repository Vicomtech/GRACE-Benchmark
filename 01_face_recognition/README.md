# Face Recognition - GRACE benchmarking dataset

The presented dataset serves for testing of face re-identification AI models and applications. It focuses on the demographic non-homogeneity of existing datasets and proposes a balanced subset of Ground Truth data in terms of three age groups (pre-pubescent, pubescent and adult) and two gender groups (male and female).

The selected corpus for this benchmark is VGGFace2, which is a large-scale face recognition dataset that includes cropped images of the head area of known celebrities, exhibiting faces with substantial variations in pose, age, illumination, ethnicity, and profession. The original dataset included over 9,000 distinct identities and over 3.3 million faces. 

For benchmarking purposes, only the Test set of the VGGFace2 corpus was selected and filtered to  ensure a balanced representation of gender and age groups, while preserving the nature of the ``in the wild" corpus, which aligns with the CSEM domain.
The resulting dataset consists of 4792 images, split between male (#2260) and femal (#2532) groups, and divided in pre-pubescent (#848), pubescent (#2255) and adult (#2093) images.

Note that the ground truth data was obtained through automatic classification employing an AI model. While errors in age or gender estimation may occur, the performance is sufficient for leveling the age and gender classes in the existing datasets so as to obtain a more homogeneous distribution and thus clearer view on the performance of face re-identification algorithms at the distinct groups.
The dataset should not be used for training person re-identification or other face characteristics AI models, nor shall it be considered for evaluating age or gender estimation models.
 

## CONTENT
The data is organised within a folder structure

### age groups: 
--- age0: pre-pubescent < 12 years
--- age1: pubescent >=12, < 18 years
--- age2: adult >= 18 years

### gender groups:
--- gender_0: male
--- gender_1: female

### occlusions groups:
--- original_images: original, non-occluded images from the VGGFAce2 dataset
--- eye_occlusion -  augmented images with artificial occlusions of the eye area
--- mouth_occlusion -   augmented images with artificial occlusions of the mouth area
--- mask_occlusion - augmented  images with respiratory masks covering mouth and nose (COVID relevant)

 ### naming convention:  
---  n000001_345_01.jpg  : identityNumber_imageNumber_counter.jpg
note that the identityNumber and imageNumber correspond to the numbers used in the original dataset
