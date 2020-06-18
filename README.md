# Informative-Image-Captioning
Image Captioning is the technique in which automatic descriptions are generated for an image. 
The entire code is in the jupyter notebook, so that should hopefully make it easier to understand. 

I have used Flickr8k dataset(size 1 GB). MS-COCO and Flickr30K are other datasets that you can use.

Flickr8K has training images-6000

validation images-1000

testing images-1000

Each image has 5 captions describing it.

For creating the model, the captions has to be put in an embedding. Setting the embedding size to 300. The image below is the model that I used.
![alt text](https://github.com/arjavdongaonkar/Informative-Image-Captioning/blob/master/model/2020-06-18%20(14).png?raw=true)

After training the model for 50 epoches with batch size of 512, 

the accuracy achived was 75% and the loss was lowered to 0.911

Finally, here are some results that I got. The code for  the results is in the jupyter notebook and you can generate your own by writing some code at the end.

1. True caption: Three child soccer players go for the ball .

![alt text](https://github.com/arjavdongaonkar/Informative-Image-Captioning/blob/master/results/2020-06-18%20(9).png?raw=true)

2. True caption: A dog wading in the water with a ball in his mouth .

![alt text](https://github.com/arjavdongaonkar/Informative-Image-Captioning/blob/master/results/2020-06-18%20(10).png?raw=true)

3. True caption: A large white bird flies over water . 

![alt text](https://github.com/arjavdongaonkar/Informative-Image-Captioning/blob/master/results/2020-06-18%20(11).png?raw=true)

4. True caption: small dog running in the grass with a toy in its mouth

![alt text](https://github.com/arjavdongaonkar/Informative-Image-Captioning/blob/master/results/2020-06-18%20(12).png?raw=true)

5.True caption: The girls is jumping into the air on the beach .

![alt text](https://github.com/arjavdongaonkar/Informative-Image-Captioning/blob/master/results/2020-06-18%20(2).png?raw=true)
