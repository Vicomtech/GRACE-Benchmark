# Named Entity Recognition - GRACE benchmark dataset

This data contains the test-set of the WNUT17 shared task (https://aclanthology.org/W17-4418.pdf), but with some extra (synthetic) noise added to the text.
The noise consists of a mixture of randomised capitalisation (some letters, or whole words, changing their capitalisation with some given probability), and randomised character-edits (addition, repetition, swap, removal of characters whitin a word).

The objective is to simulate the informal, and usually poorly written, style that one may find when digging into some online chats/forums/social-media.
This extra noise additions is far from perfect. It is just a fair attempt to check whether a system is more o less robust against this kind of text-corruption, that naturally happens in some parts of the web and dark-web.

The datasets stats and entity-types distribution is the following (the same as in the original data).

#Documents: 1287
#Tokens:    23394
#Entities:  1040
-----
  #person:        414
  #location:      139
  #corporation:   70
  #product:       127
  #creative-work: 140
  #group:         150
