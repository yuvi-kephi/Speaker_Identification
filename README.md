# Speaker_Identification
## Identifies the speaker using audio file(".wav")

This dataset contains speeches of five prominent leaders namely; Benjamin Netanyahu, Jens Stoltenberg, Julia Gillard, Margaret
Tacher and Nelson Mandela which also represents the folder names. Each audio in the folder is a one-second 16000 sample rate PCM encoded.

Originally, the speech for each speaker was a one lengthy audio, I chunked them into one-second each for easier workability. If you combine the chunked audios from 0.wav to 1500.wav, it forms a complete speech of the respective speaker.

A folder called background_noise contains audios that are not speeches but can be found inside and around the speaker environment e.g audience laughing or clapping. It can be mixed with the speech while training.

- Initially load the data set and copy the path of the folder which is downloaded.
- Use the path where to locate your respective folder
- Here we had divided the data into two phses one is for training and other for testing
we used tnesorflow, keras, numpy, shutil, pathlib and IPython, subprocess etc.., libraries 

we created a model which reads the .wav file and makes tensors matrix of it  we trained our model using conv1D and used maxpool .

further we used softmax layer as activation layer

at last optimization is done and we will trained and loded our model in .h5 extension.

Here model.h5 is used for prediction.
