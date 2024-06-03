# Age-Gender dataset - GRACE benchmarking dataset

## Description

The dataset contains images of faces, labeled for age and gender. There are 13,320 original samples, sourced from four different datasets: [UTKFace](https://susanqq.github.io/UTKFace/), [AgeDB](https://ibug.doc.ic.ac.uk/resources/agedb/), [APPA-REAL](https://chalearnlap.cvc.uab.cat/dataset/26/data/45/description/) and [IMDB](https://data.vision.ee.ethz.ch/cvl/rrothe/imdb-wiki/).


## Content

* **Original dataset** (```/original/Dataset_GRACE_AgeGender```): original images, containing human faces. Labeled for age and gender. There are 13,320 original images.
* **Dataset augmented with eye occlusions** (```/Dataset_GRACE_AgeGender_EyeOcclusions```): images from the original dataset, modified by adding black masks over the eyes.
* **Dataset augmented with mouth occlusions** (```/Dataset_GRACE_AgeGender_MouthOcclusions```): images from the original dataset, modified by adding black masks over the mouth.
* **Dataset augmented with blurring** (```/Dataset_GRACE_AgeGender_BlurFaces_s_3```): images from the original dataset, modified by blurring the faces.



### Gender

0-male, 1-female.

### Age 

There are four age groups:

* Pre-pubescent, if age is below 10 (female) or below 12 (male).
* Pubescent, if age is below 18.
* Young Adult, if age is between 18 and 25.
* Adult, if age is 26 or above.

### Distribution of the original dataset

Distribution of the samples according to the different age groups:
* 3,570 Pre-pubescent.
* 3,255 Pubescent.
* 3,242 Young adult.
* 3,253 Adult.

Distribution of the samples according to gender:
* 6,505 Male.
* 6,815 Female.

### Labels and structure of the filenames

#### Samples from UTKFace

```<age>_<gender>_<race>_<id>```

```UTK_<age>_<gender>_<id>```

Examples:

* ```89_1_0_20170110175.jpg``` --> The sample belongs to UTKFace, the person in the image is 89 years old, female.

* ```UTK_018_1_0029360.jpg``` --> The sample belongs to UTKFace, the person in the image is 18 years old, female.

#### Samples from AgeDB:

```ADB_<age>_<gender>_<id>```

#### Samples from APPA-REAL:

```APR_<age>_<gender>_<id>```

#### Samples from IMDB:

```IMD_<age>_<gender>_<id>```



