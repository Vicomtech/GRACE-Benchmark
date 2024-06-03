# GRACE-Benchmark: Standardized Corpora for Evaluating AI Tools in CSEM Investigations

The GRACE-Benchmark is a collection of curated datasets to evaluate AI tools for CSEM analysis. This is a result of the [GRACE project](https://www.grace-fct.eu/) that aimed to equip European LEAs with advanced analytical and investigative capabilities to respond to the spread of online CSEM. We explore diverse applications in CSEM investigations across various AI tasks, including, face recognition, age/gender identification,  video super resolution, speech recognition, language identification, text classification, NER, and many others.

Different processes were applied to obtain benchmark corpora for image, video, audio, and text processing applications in the context of CSEM. These processes involved data selection and augmentation strategies adapted to each application and data source. We ensured that all considered datasets were publicly available and licensed to permit derivative works.

## Image and Video Benchmarks

The GRACE benchmark datasets for Image and Video processing tools are formed by transforming source datasets to the CSEM domain. The source corpora were balanced in terms of age and gender of the persons. Data augmentation processes for these applications included image blurring and face occlusions.  

| **Image/Video Benchmark**        | **Source Datasets**                    | **Access Link** |
|----------------------------------|----------------------------------------|-----------------|
| [Face Recognition](https://github.com/Vicomtech/GRACE-Benchmark/tree/main/01_face_recognition)                 | VGGFace2                               |                 |
| [Visual Age and Gender Estimation](https://github.com/Vicomtech/GRACE-Benchmark/edit/main/02_visual_age_gender_recognition) | UTKFace, AgeDB, APPA-REAL, IMDB-Face   |                 |
| [Tattoo and Scar Detection](https://github.com/Vicomtech/GRACE-Benchmark/tree/main/03_tattoo_scar_detection)        | DeMSI                                  |                 |
| [Video Super Resolution](https://github.com/Vicomtech/GRACE-Benchmark/tree/main/04_video_super_resolution)           | REDS                                   |                 |
| [Object Detection and Recognition](https://github.com/Vicomtech/GRACE-Benchmark/tree/main/05_object_detection) | NYU Depth V2                           |                 |
| Scene Text Recognition           | ICDAR 2019                             |                 |
| Image meme/viral Detection       | Kaggle Memes, TextOCR                  |                 |
| Tampering Detection              | MISD                                   |                 |

## Audio Benchmarks

Audio benchmarks were created to evaluate each AI tool in more realistic settings, close to the CSEM domain. The process involved three strategies applied to each source dataset. The data augmentation strategies include noise addition, auddio event insertion, and child speech simulation.

| **Audio Benchmark**                     | **Source Datasets**                                                      | **Access Link** |
|-----------------------------------------|--------------------------------------------------------------------------|-----------------|
| Speech Recognition and Keyword spotting | CommonVoice, MediaSpeech, Voxforge, Spoken wikipedia corpus, Polish Parl |                 |
| Audio event detection                   | Audioset                                                                 |                 |
| Speaker Identification                  | Voxceleb                                                                 |                 |
| Acoustic Age and Gender Estimation      | NISP                                                                     |                 |
| Language Identification                 | Voxforge                                                                 |                 |
| Dialect Identification                  | CommonVoice, L2 Artic, Google Speech Resources, Voxforge                 |                 |

## Text Benchmarks

The source corpora for the text-based applications included NER, relationship extraction, and text classification. The selection and augmentation processes used to adapt each corpus to the CSEM domain involved balancing the entity types and incorporating different noise additions.

| **Text Benchmark**                      | **Source Datasets**                        | **Access Link** |
|-----------------------------------------|--------------------------------------------|-----------------|
| NER                                     | WNUT'17                                    |                 |
| Relationship extraction                 | DOCRED                                     |                 |
| Text Classification                     | DUTA                                       |                 |


## Authors

This dataset was collected within the GRACE project, by different researchers from [VICOMTECH](https://www.vicomtech.org/es/), [CERTH](https://www.certh.gr/root.en.aspx), and [GVIS](https://gvis.unileon.es/)

In partricular, the following researchers have collaborated in the dataset creation and curation process:

- Juan Camilo Vásquez-Correa
- Aitor García-Pablos
- Aitor Álvarez
- Leyanis López-Ávila
- Javier Calle-Armendariz
- Konstantinos Karageorgos
- Kassiani Zafeirouli
- Anastasios Dimou
- Petros Daras
- Alicia Martínez-Mendoza
- Andrés Carofilis-Vasco
- Enrique Alegre-Gutiérrez
- Peter Leskovský
- Arantza Del Pozo

## Contact

{jcvasquez,pleskovsky,adelpozo}@vicomtech.org

## License

To be defined

## Other relevant information

If you use this dataset, please, cite the following paper:

(INCLUDE PAPER REFERENCE WHEN PUBLISHED)
