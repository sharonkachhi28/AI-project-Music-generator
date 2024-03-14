<div id="top"></div>


<!-- PROJECT LOGO -->
<br />
<div align="center">

  <h3 align="center">music-generator</h3>

 

<!-- ABOUT THE PROJECT -->
## About The Project

<p> <img src="https://user-images.githubusercontent.com/47852354/141186269-d31ec094-8061-4edc-b862-8e1deb3da46f.png" width="600"> </p>  Generative adversarial networks have been proposed as a way of efficiently training deep generative neural networks. We propose a generative adversarial model that works on continuous sequential data, and apply it by training it on a collection of classical music. We conclude that it generates music that sounds better and better as the model is trained, report statistics on generated music, and let the reader judge the quality by downloading the generated songs.

Recently, generative neural networks have taken the stage for artistic pursuits, such as image generation and photo retouching. Another area where these deep learning networks are beginning to leave a mark is in music generation. In this project, our goal is to explore the use of **LSTM** and **GAN neural networks** to generate music that seems as if it were human-made.
By treating the notes and chords within **MIDI** files as discrete sequential data, we were able to train these two models and use them to generate completely new MIDI files. 


### Built With

Major frameworks/libraries used to this project:

* [Python 3.8](https://www.python.org/)
* [Tensorflow , Keras](https://www.tensorflow.org/)
* [Midi2audio](https://github.com/bzamecnik/midi2audio)
* [Music21](https://web.mit.edu/music21/)
* [Numpy](https://numpy.org/)



<!-- PARTS -->
## Parts

**MIDI format**
an acronym for Musical Instrument Digital Interface, a technical standard that describes a communications protocol, digital interface, and electrical connectors that connect a wide variety of electronic musical instruments, computers.


**Music21** is a powerful library in python whose tools are very helpful for creating, analysis and processing of audio files like songs, melodies and etc..
In this project, we have used this library for our purposes of converting the MIDI files into notes, categorizing of notes for preparing the training data, and choosing the playing instruments for the output of our GAN and converting it back to MIDI.


**MIDI Class:**
- Parser
- sequence preparation
- MIDI creation

**Parsing MIDI file and preparing the training data and preparing data for C-RNN-GAN network**
<p> <img src="https://user-images.githubusercontent.com/47852354/141293958-b829dce5-64e2-439b-b45b-4667608d13b6.png" width="650"> </p> 

**Model Class:**
- Discriminator
- Generator
- Train
- Plot loss function
- Save model

**Generative Adversarial Network (GAN) vs. LSTM**
<p> <img src="https://user-images.githubusercontent.com/47852354/141293644-9504c1c3-1713-4533-a91d-8e4637edd961.png" width="350">
<img src="https://user-images.githubusercontent.com/47852354/141293667-67f8be01-d6ad-4a91-8058-bb928048a771.png" width="250"> </p> 

**C-RNN-GAN Network Structure**
<p> <img src="https://user-images.githubusercontent.com/47852354/141293801-1402eb14-6e05-4ff4-a2eb-5af0abcbf239.png" width="400"> </p> 


The project has been done with aid of GPU Computing and the use of NVIDIA cuDNN and NVIDIA CUDA Toolkit. It helped us to use Tensorflow with GPU support for computing and learning with more compatibility.
The model has been trained on an **NVIDIA GeForce GTX 1080Ti GPU**.
**CUDA** is a parallel computing platform interface that allows software developers to use GPUs for ML computing.



<!-- RESULTS -->
## Results
<p> <img src="https://user-images.githubusercontent.com/47852354/141289514-87b11009-2835-407f-8cf3-dc99ed860811.png" width="300"> </p> 

https://user-images.githubusercontent.com/47852354/141285440-be56d13f-abb4-4956-9ae3-c6845ed1fd12.mov

https://user-images.githubusercontent.com/47852354/141285431-a525b350-857f-470a-9465-7935a80a06d6.mov




<!-- DATASETS -->
## Datasets

<ol>
    <li>
      GiantMIDI-Piano is a classical piano MIDI dataset contains 10,854 MIDI files of 2,786 composers. The curated subset by constraining composer surnames contains 7,236 MIDI files of 1,787 composers. GiantMIDI-Piano are transcribed from live recordings with a high-resolution piano transcription system. <a href="https://github.com/bytedance/GiantMIDI-Piano">find out more on Github</a>
      <ul>
        <li><i>Qiuqiang Kong, Bochen Li, Jitong Chen, and Yuxuan Wang. "GiantMIDI-Piano: A large-scale MIDI dataset for classical piano music." arXiv preprint arXiv:2010.07061 (2020). https://arxiv.org/pdf/2010.07061</i></li>
      </ul>
    </li>
    <li>Persian MIDI Dataset</li>
    <li>The Lakh MIDI Dataset</li>
  </ol>

