# Using RNNs to Predict the Class of Clothing in the Fashion-MNIST dataset
Created on: 10/05/2020 23:10

Updated on: 19/05/2020 13:06

# Introduction
Another important kind of Machine Learning model to explore in this series are Recurrent Neural Networks (RNNs). Recurrent Neural Networks build on the Fully Connected network idea and implement the idea of 'hidden layers', where there is a process running in parallel which accounts for factors which would typically not be included using F

# What is the Dataset?
The dataset being analysed is the Fashion-MNIST Dataset. Fashion-MNIST considers as an upgrade to MNIST to increase the difficulty of the classification problem. Fashion-MNIST is a collection of greyscale images of Fashion items, each labeled with one of ten classes:

| __Label__ | __Description__ |
|-----------|-----------------|
| 0         | T-shirt/top     |
| 1         | Trouser         |
| 2         | Pullover        |
| 3         | Dress           |
| 4         | Coat            |
| 5         | Sandal          |
| 6         | Shirt           |
| 7         | Sneaker         |
| 8         | Bag             |
| 9         | Ankle boot      |

Overall, Fashion-MNIST outlines a number of advantages over its predecessor, outlined here:

https://github.com/zalandoresearch/fashion-mnist

The fashion-MNIST dataset has a total of 60,000 points for training, 10,000 points for testing. 

# What method are we using?
Here, we are using RNN. Typically, the preferred method to analyse images are with Convolutional Neural Networks (CNNs) but we'll see how this goes. 

RNN's use a hidden layer to memorise parts of the input, allowing for more accurate predictions. This is especially helpful in applications involving text memorisation and sequence generation/prediction. What matters most in this project here is to understand the framework of building an RNN model (including the structures of a single layer in PyTorch.

In deeper models of RNNs, we encounter the issue of the earlier hidden layers having little impact on processing the latter layers, meaning that the model won't be able to identify deeply structured relationships (also known as the vanishing gradient problem). This is where LSTM's come into play. 

Long Short Term Memory networks (LSTMs), were originally developed in the late 90's by Hochreiter & Schmidhuber (1997), and are now widely used as the preferred form of RNNs. LSTM's have in-built methods to try to memorise the earlier layers of the model when computing the hidden layer, by using four separate layers which will eventually account for certain aspects of the previous set of layers. This is effectively described on the blog post: https://colah.github.io/posts/2015-08-Understanding-LSTMs/. Simplistically (and for the sake of learning this myself, I've copied the two diagrams distinguishing RNNs and LSTMs from that blog.   

One thing that I've learnt over doing this and the LSTM model is that multi-layer models are quite simple in PyTorch since you can just change the num_layers input.

# What are the results?
Initially, the RNN model was coded in a way which resulted in quite an ineffective model, with results essentially equal to random change. I wanted to use this opportunity to figure out why this was happening (since the CNN variant worked perfectly fine). 

## Part 1: Initial Modelling (with errors?)
So when trying to replicate the errors, the models turn out fine. Maybe it was something having to do with running the Anaconda session at the time?? This is a little frustrating, but it's good that the model works.

| __Epoch__ | __Iteration__ | __Loss__ | __Accuracy (%)__ |
|-----------|---------------|----------|------------------|
| 1         | 500           | 2.31     | 8.00             |
| 2         | 1000          | 2.31     | 8.00             |
| 3         | 1500          | 2.31     | 8.00             |
| 4         | 2000          | 2.31     | 8.00             |
| 5         | 2500          | 2.30     | 8.00             |

Never mind! I think I figured it out. When I was constantly running the model. I never included the criterion and optimizer back into the model, resulting in a model that wasn't learning properly. 

| __Epoch__ | __Iteration__ | __Loss__ | __Accuracy (%)__ |
|-----------|---------------|----------|------------------|
| 1         | 500           | 2.31     | 9.78             |
| 2         | 1000          | 2.30     | 9.78             |
| 3         | 1500          | 2.31     | 9.78             |
| 4         | 2000          | 2.32     | 9.78             |
| 5         | 2500          | 2.30     | 9.78             |

So if I run the model again, but with the criterion and optimizer, then I should get good results. 

| __Epoch__ | __Iteration__ | __Loss__ | __Accuracy (%)__ |
|-----------|---------------|----------|------------------|
| 1         | 500           | 2.18     | 23.18            |
| 2         | 1000          | 1.46     | 35.68            |
| 3         | 1500          | 1.19     | 50.91            |
| 4         | 2000          | 1.03     | 61.85            |
| 5         | 2500          | 1.15     | 62.14            |
| 6         | 3000          | 0.86     | 67.52            |

Fantastic! Let's run some more models, compare them (so see where the models peak, and maybe some plots too). 


## Part 2: Functional Modelling Results


## Part 3: LSTM Results


## Part 4: More Models (RNNs/LSTMs with multiple layers)


# What do we want to do moving forward?
There are still a lot of stuff for me to work on this week, a lot of it primarily involves reviewing the crime and New York location datasets. In particular, it will be worthwhile reviewing the theory associated with the models that I used to analyse that dataset at the time (Random Forests, SVR etc). It will also be extremely worthwhile to review the dataset and change it to a classification problem. 

In terms of describing the actual function of each model, I personally feel like I'd like to have more detail in why and how these models work, but this will only come when I personally get a better understanding of how they work. In future projects, I'd like to be slowly adding more detail to the model. I'm sure there will be mistakes along the way, but they will be corrected as the mistakes are identified. 

# Appendix

## Resources used:
http://www.wildml.com/2015/09/recurrent-neural-networks-tutorial-part-1-introduction-to-rnns/

https://colah.github.io/posts/2015-08-Understanding-LSTMs/

http://karpathy.github.io/2015/05/21/rnn-effectiveness/

## To-do list
- Description of Fashion-MNIST
- Sample of Fashion-MNIST (including an example of data points and labels)
- Describe how Recurrent Neural Networks work
- Describe the results
- Get a confusion matrix
- Future Directions? (Probably to do with the crime dataset)

## Template for images
<img src="images/confusion_matrix_ratio.png"
     alt="Markdown Monster icon"
     style="float: left; margin-right: 5px;" 
     width="500px;" />
