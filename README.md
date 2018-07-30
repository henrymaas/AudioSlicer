# AudioSlicer

A simple Audio Slicer in Python which can sepparate .wav audio files into multiple .wav samples, based on silence detection. Also, it dumps a .json that contains the periods of time in which the slice occours, in the following format: {sample nº : [cut start, cut end]}. Ex.:

{"0": ["0:0:0", "0:0:3"], "1": ["0:0:3", "0:0:10"], "2": ["0:10:0", "0:0:22"], "3": ["0:0:22", "0:0:32"]}

The code was taken from somewhere on GIT, but i lost the reference. I'll post it here as soon as i find it.

The filename will also contains the parts when the video were sliced, ex.: sample01_0349_0401.wav


<h2> AI Adaptation </h2>
This project will turn into a neural network which can detect audio silence and split the files.
It will also needs to learn to detect 'breathing noises' from the dictator and remove from it.



<h2> Python 3.6 - Libraries </h2>

pydub (0.22.1)

scypi (1.1.0)

tqdm (4.23.4)


<h2> Usage </h2>
To run this code, just change the path of the <b>input_file</b> and <b>output_dir</b>.
 
