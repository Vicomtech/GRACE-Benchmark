# Age and Gender estimation from audio - (GRACE benchmarking dataset)

A subset has been generated from the NISP (https://github.com/iiscleap/NISP-Dataset) dataset, by balancing the samples from the original dataset, aiming to keep a similar average age, number of speakers, and duration across genders. NISP was selected because it contains speech recordings along with speaker physical parameters (such as height or weight), regional information and linguistic information, in addition to age and gender labels. There are 345 speakers, 219 male and 126 female. The dataset contains sentences taken out from newspapers. 

|                    | Male  | Female | Total |
|--------------------|-------|--------|-------|
| Dataset            | NISP  | NISP   | NISP  |
| # Speakers         | 14    | 10     | 24    |
| Avg. Age           | 23.85 | 23.32  | 23.63 |
| # Utterances       | 1164  | 817    | 1981  |
| Total duration (h) | 2.91  | 02.08  | 4.99  |

This dataset is divided into four folders:
* clean: original audios

* background_noise: audios augmented by adding background noise from the MUSAN corpus. We added 37 background noises that are commonly found at home environments, such as eating sounds, footsteps, a coffee machine, loud TV or background music.

* children_speech: audios modified by increasing pitch and speed in order to simulate children speech. (Increasing pitch frequency between 0.25 and 0.37 semitones and increasing speed between 100 and 155% to make adult speech closer to child speech).

* event_audio: audios augmented by adding audio events from the MUSAN corpus. There are 27 categories of audio events, such as dogs barking, phones ringing, zipper sounds, breathing sounds, kitchen sounds or baby cries. We have augmented the source dataset by adding these audio events in a random position of the input audio file.

* merged: combination of all the previous augmentation techniques

The file age_gender_estimation.csv contains the labels (age and gender (F-female, M-male)) for each audio file. The audio files are identified by their path.
