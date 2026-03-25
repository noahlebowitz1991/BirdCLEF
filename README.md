# BirdCLEF

One of Kaggle's recent problems is BirdCLEF+ 2026 (https://www.kaggle.com/competitions/birdclef-2026). The project provides copious data taken from Brazil's Pantanal wetlands.
There are thousands of one minute audio files each consisting of animal noises. For each file, we also have a list of animals that appear in every 5-second increment.
There is also a list of possible animals in the files along with their class (bird, reptile, amphibian, mammal, insect).
The goal is determine the animals that appear in a files the program has not yet seen.

To start, I have made a program that determines the classes of animals that appear in a given file. Currently, the program has a 92% success rate.
More precisely, it has 100% for insects, 92% for reptiles, 99% for amphibians, 97% for mammals, and 93% for birds.
In the future, I would like to improve these results further. Once I am satisfied, I plan to look at specific animal species.
The program takes each audio file and converts it into a timeseries. It then uses PCA with dimensionality reduction for each class.
I plan to use a CNN with MEL spectrograms in future versions.

All data comes from Kaggle.

The final deadline is June 3.
