# Dialect identification dataset - Dialect/Accent detection - (GRACE benchmarking dataset)

A data subset has been generated from a combination of 5 datasets that were selected because they provide information about accents in different languages, which is a characteristic that can provide more detailed information about a speaker: CommonVoice (https://commonvoice.mozilla.org/es/datasets), L2 Arctic (https://psi.engr.tamu.edu/l2-arctic-corpus/), Google Speech Resources (Latin American Corpora) (https://github.com/google/language-resources), Voxforge (http://www.voxforge.org/es), and Portugal Police. All of them are publicly available except for the latter. The samples from this dataset are in different languages and include different accents from each language. The subset was created by balancing the samples of the original datasets, aiming to keep a similar number of utterances and duration for each accent, when possible. If the original dataset is small or contains few samples of certain accent, all the samples were included in the subset. The dataset specifications are described in the table below.

| Language   | Accent      | Base corpora           | # Utterances | Duration (h) |
|------------|-------------|------------------------|--------------|--------------|
| English    | Australia   | Common Voice           | 553          | 0.86         |
|            | Canada      | Common Voice           | 553          | 0.86         |
|            | England     | Common Voice           | 553          | 0.85         |
|            | Ireland     | Common Voice           | 550          | 0.71         |
|            | Scotland    | Common Voice           | 552          | 0.63         |
|            | Spanish     | Common Voice           | 553          | 0.78         |
|            | US          | L2 Artic               | 553          | 0.82         |
| Spanish    | Argentina   | Latin American Corpora | 1696         | 2.38         |
|            | Chile       | Latin American Corpora | 1268         | 2.02         |
|            | Colombia    | Latin American Corpora | 1493         | 2.26         |
|            | Perú        | Latin American Corpora | 1786         | 3.08         |
|            | Puerto Rico | Latin American Corpora | 186          | 0.25         |
|            | Venezuela   | Latin American Corpora | 1031         | 1.42         |
| German     | Austria     | Common Voice           | 1000         | 1.28         |
|            | Germany     | Common Voice           | 1000         | 1.54         |
|            | Switzerland | Common Voice           | 1000         | 1.64         |

This dataset is divided into four folders:

* clean: original audios

* background_noise: audios augmented by adding background noise from the MUSAN corpus. We added 37 background noises that are commonly found at home environments, such as eating sounds, footsteps, a coffee machine, loud TV or background music.

* children_speech: audios modified by increasing pitch and speed in order to simulate children speech. (Increasing pitch frequency between 0.25 and 0.37 semitones and increasing speed between 100 and 155% to make adult speech closer to child speech).

* event_audio: audios augmented by adding audio events from the MUSAN corpus. There are 27 categories of audio events, such as dogs barking, phones ringing, zipper sounds, breathing sounds, kitchen sounds or baby cries. We have augmented the source dataset by adding these audio events in a random position of the input audio file.

* merged: combination of all the previous augmentation techniques

The csv files contain the labels (language and accent) for each audio file.
