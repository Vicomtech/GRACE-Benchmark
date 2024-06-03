# Image meme/viral detection - GRACE benchmarking dataset

This dataset is created as a combination of meme images from [Kaggle's Most Viewed Memes Templates of 2018](https://www.kaggle.com/datasets/gmorinan/most-viewed-memes-templates-of-2018) and non-meme images from [TextOCR]https://www.kaggle.com/datasets/robikscube/textocr-text-extraction-from-images-dataset).

To create a balanced dataset, 10K images were chosen from each dataset. 

Additionally, a filter for face and text detection was applied to the images, because these are the most common features found in meme content.

The text files in annotations indicate if faces or  text (ocr) were detected in an image, and the coordinates of the bounding box surrounding the face or text area.

## Dataset specifications

| Dataset                     | Total number of images | Images with faces | Images with text | Images without anything |
|-----------------------------|------------------------|-------------------|------------------|-------------------------|
| Meme kaggle subset 10K      | 10,000                 | 6,077             | 9,703            | 94                      |
| Not Meme TextOCR subset 10K | 10,000                 | 3,185             | 9,058            | 646                     |
| Dataset GRACE Meme          | 20,000                 | 9,262             | 18,761           | 740                     |
