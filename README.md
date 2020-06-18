# Informative-Image-Captioning
Image Captioning is the technique in which automatic descriptions are generated for an image. 
The entire code is in the jupyter notebook, so that should hopefully make it easier to understand. 

**Dependencies**

1.Keras 1.2.2

2.Tensorflow 0.12.1

3.tqdm

4.numpy

5.pandas

6.matplotlib

7.pickle

8.PIL

9.glob

I have used Flickr8k dataset(size 1 GB). MS-COCO and Flickr30K are other datasets that you can use.

Flickr8K has training images-***6000***

validation images-***1000***

testing images-***1000***

Each image has ***5*** captions describing it.

In Image Captioning, a CNN is used to extract the features from an image which is then along with the captions is fed into an RNN. To extract the features, we use a model trained on Imagenet. I tried out VGG-16, Resnet-50 and InceptionV3. Vgg16 has almost 134 million parameters and its top-5 error on Imagenet is 7.3%. InceptionV3 has 21 million parameters and its top-5 error on Imagenet is 3.46%. Human top-5 error on Imagenet is 5.1%.

For creating the model, the captions has to be put in an embedding. Setting the embedding size to ***300***. The image below is the model that I used.
![alt text](https://github.com/arjavdongaonkar/Informative-Image-Captioning/blob/master/model/2020-06-18%20(14).png?raw=true)

After training the model for 50 epoches with batch size of 512, 

the accuracy achived was ***75%*** and the loss was lowered to ***0.911***.

Finally, here are some results that I got. The code for  the results is in the jupyter notebook and you can generate your own by writing some code at the end.

***1. True caption: Three child soccer players go for the ball .***

![alt text](https://github.com/arjavdongaonkar/Informative-Image-Captioning/blob/master/results/2020-06-18%20(16).png?raw=true)

***2. True caption: A dog wading in the water with a ball in his mouth .***

![alt text](https://github.com/arjavdongaonkar/Informative-Image-Captioning/blob/master/results/2020-06-18%20(15).png?raw=true)

***3. True caption: A large white bird flies over water . ***

![alt text](https://github.com/arjavdongaonkar/Informative-Image-Captioning/blob/master/results/2020-06-18%20(11).png?raw=true)

***4. True caption: small dog running in the grass with a toy in its mouth .***

![alt text](https://github.com/arjavdongaonkar/Informative-Image-Captioning/blob/master/results/2020-06-18%20(22).png?raw=true)

***5.True caption: The girls is jumping into the air on the beach .***

![alt text](https://github.com/arjavdongaonkar/Informative-Image-Captioning/blob/master/results/2020-06-18%20(2).png?raw=true)
