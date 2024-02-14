<h1> AudioSlicer </h1>

A simple Audio Slicer in Python that can split `.wav` audio files into multiple `.wav` samples, based on silence detection. Also, it dumps a `.json` file that contains the periods of time in which the slice occours, in the following format: 

```json
{
    "0": ["0:0:0", "0:0:3"],
    "1": ["0:0:3", "0:0:10"],
    "2": ["0:10:0", "0:0:22"],
    "3": ["0:0:22", "0:0:32"]
}
```
The file names will also contains the parts when the video were sliced, ex.: `sample01_0349_0401.wav`


<h3> Attribution </h3>

I gratefully acknowledge the original code's contribution from `/andrewphillipdoss`


<h3> AI Adaptation </h3>
This project will turn into a neural network which can detect audio silence and split the files.
It will also needs to learn to detect 'breathing noises' from the dictator and remove from it.


<h2> Requirements: </h2>

+ Python 3.11.0
+ numpy - 1.24.1
+ scypi - 1.10.0
+ tqdm - 4.64.1


<h2> Usage </h2>

1. Edit `AudioSeg.py` and change the <b>input_file</b> (full path to your original .wav file) and <b>output_dir</b> (folder path to the destination of the audio splits).
2. Run python -m AudioSeg.py
<br/><br/>

> [!NOTE]
> Please note that in order for your audio file to be cut into samples, it should contain periods of "silence". If you are trying to extract voice samples from a song, for example, it may not work as expected.
<br /><br />
>Depending on the level of noise in your audio, the algorithm may skip the silence windows, resulting in missed cuts. Ensure that your audio is free from unwanted noise and that the silences are clearly defined. You can adjust the parameters of >> 
<b>min_silence_length</b>, <b>silence_threshold</b>, and <b>step_duration</b> to modify the length, amplitude, and duration of the silence window in order to better match your audio
