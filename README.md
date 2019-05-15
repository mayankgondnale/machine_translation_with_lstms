# Speech Recognition and Machine Translation using Sequence to Sequence Models

The idea is to use sequence-to-sequence Recurrent Neural Networks to translate from one language to another. The input sequence is passed through a RNN to obtain the output sequence. The model is flexible such that the lengths of the input sequence and the output sequence can differ. A Speech Recognition layer has also been added on top of the translation framework. 
The speech recognition layer takes in live speech as input and transcribes it into text which is further treated as the input sequence for the many-to-many RNN which gives the output sequence in the desired langauge.

The architecture could be understood by the below image -

![](images/architecture.JPG)

The training data is a 2-column dataset - column 1 containing words/phrase in input language (English) and column 2 containing translations of those in column 1 in the output language (German). Since column 2 is the exact translation of column 1, this takes into account all the grammar rules and patterns.
The dataset has been obtained from - http://www.manythings.org/anki/.

![](images/file.JPG)

