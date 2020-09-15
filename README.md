<h1>Goldberg Variation 31</h1>
<br>
<p><em>Goldberg Variations (BWV 988)</em> is a set of 30 variations based on an original aria written for the keyboard by Johann Sebastian Bach in the year 1741.<br>
  In this repository, I have created a 31st Goldberg variation using Recurrent Neural Networks.<br>
  Three different datasets have been used to create three different variations to Bach's aria.
<br>
  MelodyRNN has been used to produce output sequences. The datasets are in MIDI format.<br>
  </p>
  
  <h2>About The Procedure</h2>
  <h3>Code</h3>
  <p>The code used has been provided in this file <a href="https://github.com/sakethram88/Goldberg_DeepLearning/blob/master/Goldberg_DeepLearning.ipynb">Goldberg_DeepLearning.ipynb</a><br>
  <a href="https://magenta.tensorflow.org/"> Magenta </a> is an open source python library which can be used to generate music and art using machine learning.
  <br>MelodyRNN can be used to generate melodies. It is an LSTM based neural network.
  <br>
  MelodyRNN works on Note Sequences but our datasets are in MIDI format, so some functions have been used to facilitate interconversion between them.<br></p>
  
  <h3>Datasets</h3>
  <p>
  Three different outputs have been generated using three different datasets from Bach's original work. <br>
  The first dataset is the complete aria.<br>
  The second dataset is the aria split into 32 different files, each containing 1 bar of music from the aria.<br>
  The third dataset has been rearranged such that a single file contains music with the same key structure from different variations. For example, the first file contains music from the first bar of aria, variation 1, variation 5, etc. <br>
  All data has been normalised to a tempo of 108 BPM and same dynamic marking for consistency.
  </p>
  
  <h3>Generation</h3>
  <p>Output has been generated as a single 32-bar MIDI file from the first dataset.<br>
  From the second and third datasets, each output contained one bar of music. All these bars were put together manually to generate the variation.<br>
  All the generated MIDI files lacked key signatures and had a 4/4 time signature. <br>
  All changes to the scores, datasets and outputs were made using the software <em>Harmony Assistant.</em><br>
  During output generation, <em>temperature</em> parameter was adjusted to alter the randomness of each output.<br>
  In general, it was observed that a log-likelihood of -400 to -450 produced intelligible results.</p> 
  <h2>Outputs</h2>
  <h3><a href="https://github.com/sakethram88/Goldberg_DeepLearning/tree/master/Dataset%201">Dataset 1</a></h3>
  <p>Dataset 1 contains the commplete aria.<br>
  This was provided as input to the code.<br>
The following output was obtained</p>
<img src="https://github.com/sakethram88/Goldberg_DeepLearning/blob/master/Dataset%201/Dataset%201%20Output/Dataset%201%20Output%20Score/Dataset%201%20Output.png" style="border:10px;">

  
