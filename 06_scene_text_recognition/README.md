# Scene Text Recognition - GRACE benchmarking dataset

## Description

The benchmark dataset for scene text recognition is created to evaluate models trained to differentiate between images containing or lacking text, 
allowing text-bearing images to be further analysed using optical character recognition (OCR). The ICDAR2019 dataset was employed as the source data, 
as it includes a broad spectrum of languages and text sizes.
The GRACE benchmark corpus is then composed by images with text in various languages/alphabets, text formats, and sizes. 
This variety enables trained models to effectively identify and classify text in real-world scenarios, where text may appear in different languages or formats.


The 10,000 images are ordered in the dataset such that each consecutive 1000 images contain text of one main language (and it may of course contain additional text from 1 or 2 other languages, all from the set of the 10 languages)
00001 - 01000:  Arabic
01001 - 02000:  English
02001 - 03000:  French
03001 - 04000:  Chinese
04001 - 05000:  German
05001 - 06000:  Korean
06001 - 07000:  Japanese
07001 - 08000:  Italian
08001 - 09000:  Bangla
09001 - 10000:  Hindi

We also covered images that are obtained from indoor (5528) and outdoor (4468) scenarios, and those displaying small (area<2000 pixels), medium (2000 < area < 10000 pixels), and large (area>10000 pixels) texts.



|Language | Words | Indoor | Outdoor | Small | Medium | Large |
|---------|-------|--------|---------|-------|--------|------|
|Arabic  | 427 | 557 | 3891 | 3286 | 2357 |
|English  | 438 | 544 | 5390 | 1957 | 1408 |
|French  | 615 | 385 | 1209 | 1279 | 3145 |
|Chinese  | 388 | 612 | 1246 | 1879 | 2744 |
|German  | 528 | 472 | 5701 | 1859 | 3340 |
|Korean  | 790 | 210 | 6119 | 2848 | 5083 |
|Japanese  | 626 | 374 | 7974 | 2137 | 3778 |
|Italian  | 615 | 385 | 22611 | 5530 | 4714 |
|Bangla  | 658 | 342 | 437 | 1208 | 4007 |
|Hindi  | 409 | 547 | 888 | 1565 | 1945 |




## Content

* **Clean dataset** (```/Clean/```): original images.
* **Blurred_k5_s1** (```/Blurred```): Blurred images.
* **Labels** (```/labels```): Text label for each image.
* ```scenarios.csv```: Indicator whether the image was taken indoor or outdoor.


