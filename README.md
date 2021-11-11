# Tensorflow-Simple-Tree-Recognition
During lockdown with all the extra time I was able to spend more of it in nature and develop my knowledge about trees

started to redisover nature, expanded my knoweldge about treees and shit. Wanted to try a AI thing on trees in my local woods so chose some of my favourites aswell as having some variety in trees chosen also quite simple in that doesnt do exact species

TOok some photos to create own dataset 

started with Alexnet and tried to get it to work better

Did this in variuous angles, light settings, zoomed in etcetc to try and get some variation in the dataset aswell as variations in tree age

As seen on the confusion matrix in the notebook - redwood, fir, pine, and birch are all quite distinctive and easy to recognise, but the NN struggles for oak, larch, pine, and poplar. The NN almost completley accuratley predicts poplars as poplars but it also consistently mislabels oaks and larches as poplars aswell. Looking at photos of these trees it can be quite easy to see why, these have quite similar bark strucutres, whereas something like the redwood is very distinctive in texture as well as colour.



Solarized dark             |  Solarized Ocean
:-------------------------:|:-------------------------:
![](https://...Dark.png)  |  ![](https://...Ocean.png)



Issues:
some young to old age trees look super different ie the douglas fir
no young poplars in woods so this app isnt very general
big variation in trees so makes it easier
think redwood easy to spot cus very red
hard to tell differences between poplars and oak and another one as can be seen on the confusion matrix

bad accuracy but realised when I indentify a tree i look at its branches/leaves as well as bark so thats improvement to make



## Next Steps:
* Take more photos for the dataset, hopefully this will greatly increase the NN performance
* Further work developing the NN to enable better learning, reducing the overfitting whilst reataining the train set accuracy
* As seen in the commented out sections of the code I want to try masking to removed backgrounds and the sky to try to focus the image by its bark, currently difficult since barks are such varying colours
* Add another network focusing on images of the canopy and then combining the percentage results from each network to get a better total accuracy for a combination of a picture of bark and a photo of the canopy



