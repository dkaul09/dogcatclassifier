# dogcatclassifier

<ins> **Project Description** </ins>

I built A dog and cat classifier, using on TensorFlow, that has been trained on the 25,000 images of dogs and cats provided by Kaggle. (The 25,000 dataset that I have used to trained the model can be found at this link: https://www.kaggle.com/competitions/dogs-vs-cats/data ) 


I have also uploaded a folder of sample test images that can be used to perform testing of this model. 

As for the kernel, I was not able to upload it due to its large image size, but I created a virtual enviornment and associated the kernel with it. 

<ins> **My Experience Building this project** </ins>

This is one of my first Machine Learning projects I have built. Having watched multiple Machine Learning tutorials during this summer, I decided to apply the concepts I have learnt through them into building a project. 

Overall, while I had some initial challenges and some improvements to make, I enjoyed building this project as it was nice to see all the concepts that I have learned come to play, allowing me to understand their significance in machine learning projects. This was a great self-learning experience and I am looking forward to taking the lessons I have learnt to make my next machine-learning project bigger and better - a dog breed classifier.


<ins>**How I overcame some challenges I faced and what I would like to improve on**</ins>

The biggest thing I want to improve is my understanding of models and I believe that will come with experience of building machine - learning projects. I have tried studying what the individual functions in the model, but I do not fully understand everything, hence I took the model in my project from the video referenced in the steps. Nonetheless, this is something I will continue working on as I continue building more machine-learning projects. 

Another issue I faced was trying to reduce the loss for the validation data. I noticed that my model was extremely overfitting at one point as majority of the images I tested the model on would always misidentify that image. I managed to reduce the severity of the issue by lowering the number of epochs and batches. However, there is still some overfitting present as the validation loss kept increasing instead of decreasing while I was training the model. This is one issue I will work towards avoiding when working on my next machine-learning project.

<ins>**How does the project work?**</ins>

1. First, I imported all the required libraries.
   ![image](https://github.com/dkaul09/dogcatclassifier/assets/111927365/28625d61-c5f1-4b0b-8c9d-69f0e211118b)
2.  I then generate a dataset from the image files in the directory. Next, I call a batch of the images and as seen below there are pictures of both cats and dogs. The number 0 represents cats while 1 represents dogs.
   ![image](https://github.com/dkaul09/dogcatclassifier/assets/111927365/e20bc4db-56f5-4f66-a608-acb4365d75f5)
3. I scale the images at this step by dividing the pixel values by 255. Scaling is important as it helps improve the training model's performance and normalizes the range of data.
   ![image](https://github.com/dkaul09/dogcatclassifier/assets/111927365/6acd7395-55b7-4f17-886a-31699715d452)
4. Below I am establishing the size of the training data, validation data, and testing data as 0.7,0.2,0.1 respectively. I chose these values to reduce possibility of overfitting.
   ![image](https://github.com/dkaul09/dogcatclassifier/assets/111927365/159aad37-d9cd-40e3-bd97-8c87258aadc2)

5. Down below is the architecture of the model. I was not familiar with how to build and design models (more on this later) so I used the models used in this video (https://www.youtube.com/watch?v=jztwpsIzEGc&t=3218s)

![image](https://github.com/dkaul09/dogcatclassifier/assets/111927365/3ed338f8-709c-4906-ac81-27f0f4209531)

6. The model gets trained here.
   ![image](https://github.com/dkaul09/dogcatclassifier/assets/111927365/d383d51e-7540-483c-8277-720954fd4c0c)

7. Below are graphs of the losses and accuracies of the training data and the validation data. (Ideally the losses for the validation data should go down as mentioned in the improvements section).
   ![image](https://github.com/dkaul09/dogcatclassifier/assets/111927365/8c69c0e2-e75b-42df-99f8-1a671358329a)

8. We are now testing the model on the test data established earlier.
   ![image](https://github.com/dkaul09/dogcatclassifier/assets/111927365/0c1de400-a03a-4da4-a7a8-46213b015727)

9. This final stage is where I load up a picture of a cat and transform it and rescale it to the model to predict. The model identifies that it is a cat.
    ![image](https://github.com/dkaul09/dogcatclassifier/assets/111927365/75a12b6e-ffb8-4f27-869f-fdd04bd08cb2)
   ![image](https://github.com/dkaul09/dogcatclassifier/assets/111927365/a6bddad3-e432-4e6e-98ad-560d2bc932b9)





