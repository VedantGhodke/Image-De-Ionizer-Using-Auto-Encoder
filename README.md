# Image De-Ionizer Using Auto-Encoder
<br>
This projects tries to replicate a popular technique known as image de-ionising i.e: noise removal from images. It uses a convolutional auto-encoder which is able to remove noise from a fed image.

# Auto-Encoder:
<br>
Auto-Encoder is an unsupervised learning technique which learns pixel-to-pixel mapping. It consists of an encoder-decoder network, of which encoder tries to compress the image to extract useful features and the decoder reconstructs the image.
<br>
However, the prevalent issue with autoencoders is that, the quality of output image is not detailed. The reasons being, we are forcing the encoder (the last layers) to learn features of the entire image, the decoder uses this encoding to reconstruct the image. As the features provided were less, so is the quality. 

# Approach:

I have designed a bot-tool for stone-paper-scissors. <br><br>
Please find the tool repository here : <a href="https://github.com/VEDANTGHODKE/Stone-Paper-Scissors-Robot-Using-Keras-and-OpenCV">"Stone-Paper-Scissors Bot by Vedant Ghodke"</a>
I have employed this model for the fine-tuning of the dataset I have used for the stone-paper-scissors bot. I have provided the dataset used in the above project in this repository. However, the above presented repository for the bot contains the code for training the model. I have taken those images, resized them and have added noise to them. The image containing noise is fed as input and the same images without noise are used for 'y_labels'.<br>
We can add noise to the images using OpenCV. For loading, resizing, and saving of images, I have used OpenCV.<br>
I have used Keras for training the auto-encoder model.
# Input and Output Images:
![scissor](https://user-images.githubusercontent.com/24778913/45904332-5b914e80-be0a-11e8-9b47-c53eda638f92.png) <br>
![paper](https://user-images.githubusercontent.com/24778913/45904370-6fd54b80-be0a-11e8-8596-f517879b74c4.png) <br>
![stone](https://user-images.githubusercontent.com/24778913/45904389-84b1df00-be0a-11e8-8923-91d1934b17ae.png) <br>

## Requirements:
1. Python 3.0
2. <a href="https://tensorflow.org">TensorFlow 2.0</a>
3. <a href="https://keras.io">Keras</a>
4. OpenCV 4.0 (for loading, and resizing images)
5. h5py (for saving trained model)
6. pyttsx3

## Installation of Requirements:
1. Start your terminal or 'CMD' (depending on your OS).
  2. If you do have an Nvidia GPU, then make sure you have the pre-requisites satisfied for Tensorflow GPU installation. Thereafter use the following commmand:

    pip install -r requirements_gpu.txt

  3. In case you do not have a GPU, then use the following command:

    pip install -r requirements_cpu.txt
  
<br>
## Steps to execute the repository:

1) Clone the repository locally<br>
2) Extract the data folders<br>
3) Install the requirements<br>
4) You can change the name of test image in runner.py<br>
5) Run "runner.py" script


## References
1) Deep Learning with Python - Francois Chollet<br>
2) Keras (Official Documentation)<br>
3) Pyimagesearch.com - Adrian Rosenberg

