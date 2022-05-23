# Deep Learning Emotion Detection

A deep learning aplication,  using CNNs to develop a solution for a classification problem, namely the emotion recognition task. <br />
Data-set used: https://www.kaggle.com/datasets/msambare/fer2013 <br />
  

## Methodology

- Trained CNN with the FER-2013 <br />
- Used a video as a prediction input <br />
- Recognise the face from the video <br />
- Detect the emotion of the frame<br />

## CNN architecture

Sequential model1:
  - Conv2D (3, 3) with 32 Channels, activation with relu
  - Conv2D (3, 3) with 64 Channels, activation with relu
  - MaxPooling2D (2, 2)
  - Dropout
  - Conv2D (3, 3) with 128 Channels, activation with relu
  - MaxPooling2D (2, 2)
  - Dropout
  - Conv2D (3, 3) with 256 Channels, activation with relu
  - MaxPooling2D (2, 2)
  - Dropout
  - Flatten
  - Dense with 512 Channels, activation with relu
  - Dropout
  - Dense with 7 Channels, activation with softmax

  Sequential model2
  - Conv2D (3, 3) with 32 Channels, activation with relu
  - BatchNormalization
  - MaxPooling2D (2, 2)
  - Conv2D (3, 3) with 64 Channels, activation with relu
  - BatchNormalization
  - MaxPooling2D (2, 2)
  - Conv2D (3, 3) with 128 Channels, activation with relu
  - BatchNormalization
  - MaxPooling2D (2, 2)
  - Conv2D (3, 3) with 256 Channels, activation with relu
  - BatchNormalization
  - MaxPooling2D (2, 2)
  - Flatten
  - Dense with 128 Channels, activation with relu
  - BatchNormalization
  - Dense with 256 Channels, activation with relu
  - BatchNormalization
  - Dense with 7 Channels, activation with sigmoid

  Sequential model3:
  - Conv2D (4, 4) with 64 Channels, activation with relu
  - BatchNormalization
  - Conv2D (4, 4) with 64 Channels, activation with relu
  - BatchNormalization
  - MaxPooling2D (2, 2)
  - Droupout(0.2)
  - Conv2D (4, 4) with 128 Channels, activation with relu
  - BatchNormalization
  - MaxPooling2D (2, 2)
  - Droupout(0.3)
 
  - Conv2D (4, 4) with 128 Channels, activation with relu
  - BatchNormalization
  - Conv2D (4, 4) with 128 Channels, activation with relu - BatchNormalization 
  - MaxPooling2D (2, 2)
  - Droupout(0.4)
  - Flatten
  - Dense with 128 Channels, activation with linear
  - Dense with 7 Channels, activation with softmax

Optimizer : Adam
Loss : Categorical Crossentropy


## Installation
The program is in Python <br />
The CNN is build with keras library <br />
The video is processing with OpenCV <br />

## Contributors
Elena Kane </br>
Borislava Sandeva <br />
