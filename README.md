# BirdCLEF

One of Kaggle's recent problems is BirdCLEF+ 2026 (https://www.kaggle.com/competitions/birdclef-2026). The project provides copious data taken from Brazil's Pantanal wetlands.
There are thousands of one minute audio files each consisting of animal noises. For each file, we also have a list of animals that appear in every 5-second increment. These files can contain the sounds of multiple types of animals. On top of this, we have around 60,000 audio files consisting of one type of animal.
There is also a list of possible animals in the files along with their class (bird, reptile, amphibian, mammal, insect).
The goal is determine the animals that appear in a files the program has not yet seen.

At this point, the model in best_multilabel_model.keras determines the animal classes in a given audio file with 99.1% accuracy. For code that generates this model, see animal_class_classifier.ipynb. The program takes each audio file and converts it into a timeseries. It then converts the timeseries to MEL spectrograms and applies a multilabel CNN.

The individual animal classes have their own separate models.

All data comes from Kaggle.

The final deadline is June 3.
