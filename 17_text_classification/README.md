# Text Classificatrion - GRACE bencmarking dataset

## Files

* DUTA_10K_original
* DUTA_augmented_change_one_word_randomly
* DUTA_augmented_change_one_word_synonym
* DUTA_augmented_change_random_word_place
* DUTA_augmented_noise_addition

The original samples (DUTA_10K_original) are from the DUTA dataset (https://gvis.unileon.es/datasets-duta-10k/). 10K web domains scraped from the Tor network. Each domain is a web page. It is divided into suspicious (illegal) activities and normal (legal)
activities. The suspicious activities are drugs, violence, counterfeit credit cards, and pornography, including 105 samples related to CSEM.

## Types of augmentation

The data augmentation was added to simulate noise found in informal text (chats, social media...)

* DUTA_augmented_change_random_word_place: Change the place of a word. A random word is moved to a different place inside the sentence. Example: “This sentence is an example” becomes “This is an example sentence”.

* DUTA_augmented_change_one_word_synonym: Change words by a synonym. A random word is replaced by a synonym. Example: “This house is great” becomes “This house is awesome”.

* DUTA_augmented_change_one_word_randomly: Change a word randomly. A word in the sentence is replaced by another random word. Example: “This is a sentence example” becomes “This is a cat example”.

* DUTA_augmented_noise_addition: Noise addition. Adds noise randomly. The types of noise that can be added are: removing capitalization, capitalize a complete word, duplicating a character, removing a character, replacing a character by another random character, and swapping characters. Example: “this is a text written very nicely as an Example , mentioning Barack Obama and Washington” becomes “THIS Is a text wriTten vyry nicely as an ExAmple , mentioning Barack OBAMA and Washington”.
