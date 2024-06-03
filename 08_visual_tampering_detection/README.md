# Visual tamper detection dataset  - GRACE benchmar dataset

The source dataset selected for visual tamper detection is the Multiple Image Splicing Dataset ([MISD](https://doi.org/10.5281/zenodo.5525829)). It contains tampered images, generated using crop-paste ooperation under Adobe Photoshop on the orignial images. There are 462 tampered images, that we filtered using face detection and text detection methods. 

The dataset has been filtered and divided into four different folders:
* images_with_face: images from MISD dataset that contain faces
* images_with_ocr: images from MISD which contain text
* images_without_anything: images from MISD which do not contain faces or text

The annotation files contain the following columns:
    Name of the image
    Type of annotation (face/ocr)
    Top-left x-coordinate of the bounding box
    Top-left y-coordinate of the bounding box
    Width of the bounding box
    Height of the bounding box
For example:
000008.jpg face 54 61 79 118
000008.jpg ocr 7 -1 76 20
000008.jpg ocr 143 2 35 19

Note that if an image contains both faces and text, it will be in both folders (images_with_face and images_with_ocr).


The ground truth masks of the images are included in the file ```Ground_Truth_Masks```.

## Dataset specifications

|                                       | Number of images |
|---------------------------------------|------------------|
| All tampered images                   | 462              |
| Tampered images with faces            | 175              |
| Tampered images with text             | 13               |
| Tampered images without faces or text | 279              |
