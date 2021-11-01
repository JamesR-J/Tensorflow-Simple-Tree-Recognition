# Tensorflow-Simple-Tree-Recognition
During lockdown with all the extra time I started to redisover nature, expanded my knoweldge about treees and shit. Wanted to try a AI thing on trees in my local woods so chose some of my favourites aswell as having some variety in trees chosen also quite simple in that doesnt do exact species

TOok some photos to create own dataset 

Did this in variuous angles, light settings, zoomed in etcetc to try and get some variation in the dataset aswell as variations in tree age

Issues:
some young to old age trees look super different ie the douglas fir
no young poplars in woods so this app isnt very general
big variation in trees so makes it easier
think redwood easy to spot cus very red
hard to tell differences between poplars and oak and another one as can be seen on the confusion matrix

bad accuracy but realised when I indentify a tree i look at its branches/leaves as well as bark so thats improvement to make



## Next Steps:
* Further work developing the NN to enable better learning.
* Rather than 3 set actions have a vector space to decide how far to turn the boat left or right
* Create boat inertia so that the boat doesn't just stop when it is turning
* Inverse RL - it would be an interesting idea to see what reward criteria this method creates and whether it would improve model performance
* Dynamic wind direction and speed
* Add the ability to foil, will add further complexity as foiling is dependant on boat velocity being great enough

want to add masking to try and remove background or sky etc
add stuff for identificing canopy pictures
better NN with reduced overfitting without reducing accuracy

