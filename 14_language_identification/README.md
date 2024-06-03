# Language Identification dataset - (GRACE benchmarking dataset)

A test set was extracted from the Voxforge (http://www.voxforge.org/es) dataset, by balancing the samples of the original dataset, aiming to keep a balance between utterances and duration for each language. The audios in this dataset were recorded from volunteers and it was selected because of the variety of languages that it contains.

The dataset distribution is shown in the table below.

| Language   | # Utterances | Duration (h) |
|------------|--------------|--------------|
| German     | 1485         | 2.29         |
| Dutch      | 826          | 1.35         |
| French     | 1723         | 2.99         |
| English    | 1981         | 3.21         |
| Greek      | 416          | 1.18         |
| Italian    | 1567         | 2.96         |
| Portuguese | 148          | 0.19         |
| Russian    | 1309         | 3.19         |
| Spanish    | 1078         | 2.45         |
| Ukrainian  | 70           | 0.18         |


This dataset is divided into four folders:
* clean: original audios

* background_noise: audios augmented by adding background noise from the MUSAN corpus. We added 37 background noises that are commonly found at home environments, such as eating sounds, footsteps, a coffee machine, loud TV or background music.

* children_speech: audios modified by increasing pitch and speed in order to simulate children speech. (Increasing pitch frequency between 0.25 and 0.37 semitones and increasing speed between 100 and 155% to make adult speech closer to child speech).

* event_audio: audios augmented by adding audio events from the MUSAN corpus. There are 27 categories of audio events, such as dogs barking, phones ringing, zipper sounds, breathing sounds, kitchen sounds or baby cries. We have augmented the source dataset by adding these audio events in a random position of the input audio file.

* merged: combination of all the previous augmentation techniques

In addition, the file test_set_new_dir.csv contains the following columns:

* Original Path to each audio file

* Duration of each audio file

* Speaker present in each audio

* Language of each audio file

* New path of each audio file
