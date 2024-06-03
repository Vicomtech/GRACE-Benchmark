# Speaker Identification dataset - (GRACE benchmarking dataset)

We have selected all the audios from the test set of the original VoxCeleb 1 (https://www.robots.ox.ac.uk/~vgg/data/voxceleb/vox1.html) dataset, since they were recorded in a wide variety of real-world conditions. 

The test set is composed of pairs of audios, where the speaker identification model will determine if the same speaker is present in each pair of audios. This dataset contains audios from 40 different speakers, is composed of 9,414 utterances and has a total duration of 172.96 hours as it can be seen in the following table.

| Dataset            | VoxCeleb 1 |
|--------------------|------------|
| # Speakers         | 40         |
| # Videos           | 674        |
| # Utterances       | 9414       |
| Total duration (h) | 172.96     |

This dataset is divided into four folders:
* clean: original audios

* background_noise: audios augmented by adding background noise from the MUSAN corpus. We added 37 background noises that are commonly found at home environments, such as eating sounds, footsteps, a coffee machine, loud TV or background music.

* children_speech: audios modified by increasing pitch and speed in order to simulate children speech. (Increasing pitch frequency between 0.25 and 0.37 semitones and increasing speed between 100 and 155% to make adult speech closer to child speech).

* event_audio: audios augmented by adding audio events from the MUSAN corpus. There are 27 categories of audio events, such as dogs barking, phones ringing, zipper sounds, breathing sounds, kitchen sounds or baby cries. We have augmented the source dataset by adding these audio events in a random position of the input audio file.

* merged: combination of all the previous augmentation techniques

The file speaker_processing_audios.csv contains information about the audio files (path, speaker, duration) and file veri_test2.txt contains the comparison between each pair of audios and the label indicating if they belong to the same speaker (1) or to different speakers (0). 
