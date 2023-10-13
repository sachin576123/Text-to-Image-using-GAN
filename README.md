
# Text to Image Generation

Text to Image Generation is a project that uses deep learning, specifically Generative Adversarial Networks (GANs), to convert text descriptions into corresponding images. This technology allows for the creation of visual content based on textual input, finding applications in areas like art, design, and content generation.  
The challenge I aimed to address was the generation of realistic images of flowers based on textual descriptions. The task involved teaching a machine to understand flower-related 
language and translate it into different visual representations, contributing to applications in art, design, and more."
ex:the flower has dark black petals and the center of it is brown and has black pistil"



## Key Features
Text to Image Generation is a process where you convert textual descriptions into corresponding images. This project leverages Generative Adversarial Networks (GANs) to achieve this task. Here's a step-by-step explanation of how the system operates:
### 1.Data Preparation: 
To train a GAN for text-to-image generation, you first need a dataset containing pairs of text descriptions and corresponding images. These pairs are used to teach the model how to generate images based on textual descriptions.
 - Oxford 102 Flowers Dataset : It is a 102 category dataset, consisting of 102 flower categories. The flowers chosen to be flower commonly occuring in the United Kingdom. Each class consists of between 40 and 258 images. It consists of 8136 images.


### 2.Text Embedding: 
The process starts with encoding the textual description into numerical format that a is often done using techniques like word embeddings as a Word2Vec, Recurrent Neural Networks (RNNs) ,where each word in 
the description is represented as high-dimensional vector.

### 3.Conditional GAN: 
This project likely uses a conditional GAN (cGAN) architecture. In a cGAN, both the text embeddings and random noise vectors are provided as input to the generator network. The generator uses the text embeddings as a condition to generate images that match the textual description.

### 4.Generator: 
The encoded text is then fed into a generator netowork.The generator is responsible for producing images from the provided text embeddings and random noise.The generator network consists of layer that learn to transform the encoded
text reprensentation into visual features and details that correspond to the description.It may consist of convolutional layers and upsampling operations to progressively generate more complex visual features.

### 5.Discriminator: 
The discriminator is another neural network that evaluates how well the generated image matches real images. It distinguishes between real and generated images. During training, the generator aims to produce 
images that can fool the discriminator.

### 6.Training: 
The cGAN is trained through a competitive process. The generator tries to produce images that the discriminator cannot distinguish from real images, while the discriminator improves its ability to differentiate 
between real and generated images. This adversarial training process continues until the generator becomes proficient at creating realistic images from textual descriptions.




## GAN
Generative Adversarial Network (GAN) is a class of machine learning
systems in which two neural networks contest with each other in a
zero-sum game framework. It consists of two networks ,One neural
network,called the generator, generates new data instances, while the other, the discriminator,evaluates them for authenticity.
  ![image](https://github.com/sachin576123/Learning-Management-System/assets/33089431/e12e4966-5ff8-4981-b4b8-1798ed7cf91b)
  
 - 1.The generator takes in random numbers and returns an image.
 - 2.This generated image is fed into the discriminator alongside a stream of images taken from the actual, ground-truth dataset.
  - 3.The discriminator takes in both real and fake images and returns probabilities, a number between 0 and 1, with 1 representing a prediction of authenticity and 0 representing fake.
  - 4.The discriminator is in a feedback loop with the ground truth of the images, which we know.
  - 5.The generator is in a feedback loop with the discriminator.

  ![image](https://github.com/sachin576123/Learning-Management-System/assets/33089431/34ba9639-eca3-4042-903d-9683a37a9ea5)
## Result
Below we display the results we got from our model on the following text queries:
 - 1.The flower shown has yellow anther blue pistil and yellow petals.
  - 2.this flower has petals that are white, and has dark lines
  - 3.the petals on this flower are pink with a dark center.
  - 4.this flower has a lot of small round blue petals.
  - 5.this flower is red color petals.
  - 6.the flower has dark black petals and the center of it is brown and has black pistil.
   - 7.the flower shown has green petals with dark center green  anther green pistil.
   - 8.these white flowers have petals that start off white in color and end in a white towards the tips

   ![image](https://github.com/sachin576123/Learning-Management-System/assets/33089431/12912263-f067-43e9-a622-d62f26a77dec)

## Tech Stack

**Language:** Python

**Techniques :** Deep Learning , Natural Language Processing

**Framework:** TensorFlow
## Learning
 Through this project ,I gained a deeper understanding of GAN archotecture , natural language processing and the intricacies of training model for creative task. I also learned to address challenges like 
 text-to-image consistency and maintaining the quality of generated images.


## Support

For support, email sachin576123@gmail.com.

