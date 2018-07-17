# AudioSlicer

A simple Audio Slicer in Python which can sepparate .wav audio files into multiple .wav samples, based on silence detection.
The code was taken from somewhere on GIT, but i lost the reference. I'll post it here as soon as i find it.


# Further Adaptation
I'm adapting it to show at which point of the video (period of time) the slicing occours, ex.: sample 1 - 03:49 to 04:01

The filename will also contains the parts when the video were sliced, ex.: sample01_0349_0401.wav


# AI Adaptation
This project will turn into a neural network which can detect audio silence and split the files.
It will also needs to learn to detect 'breathing noises' from the dictator and remove from it.



# Python 3.6 - Libraries

pydub (0.22.1)

scypi (1.1.0)

tqdm (4.23.4)

