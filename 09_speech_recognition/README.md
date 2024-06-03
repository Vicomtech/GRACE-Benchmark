# Speech Recognition and Keyword spotting - GRACE benchmark dataset

The source datasets for this tool are formed with audio and transcripts in seven languages, covering English, Spanish, German, French, Italian, Portuguese, and Polish.


The source dataset to create this benchamrk is based on: CommonVoice, MediaSpeech, Voxforge, Spoken wikipedia corpus, Polish Parl. 

The test sets from these source corpora were filtered based on the presence of a list of CSEM-related keywords (**keywords.csv**).

Finally, the selected audios were augmented by adding background noise, inserting audio events, and smulating child speech.


## Dataset specifications

| Language | Source corpora            | N utterances | Duration (h) |
|-------------------|-------------------------------------|------------|------------|
| English           | Common Voice, SWC                   | 4096       | 11.3       |
| Spanish           | Common Voice, MediaSpeech, Voxforge | 1449       | 3.5        |
| German            | Common Voice, Voxforge, SWC         | 1226       | 3.7        |
| French            | Common Voice, MediaSpeech, Voxforge | 2636       | 6.3        |
| Italian           | Common Voice, Voxforge              | 3279       | 6.2        |
| Portuguese        | Common Voice, Voxforge              | 702        | 1.1        |
| Polish            | Common Voice, Polish parliament     | 711        | 1.3        |
