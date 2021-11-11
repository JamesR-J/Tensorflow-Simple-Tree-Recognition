# Tensorflow-Simple-Tree-Recognition
During lockdown with all the extra time I was able to spend more of it in nature and develop my knowledge about trees

started to redisover nature, expanded my knoweldge about treees and shit. Wanted to try a AI thing on trees in my local woods so chose some of my favourites aswell as having some variety in trees chosen also quite simple in that doesnt do exact species

TOok some photos to create own dataset 

started with Alexnet and tried to get it to work better

Did this in variuous angles, light settings, zoomed in etcetc to try and get some variation in the dataset aswell as variations in tree age

As seen on the confusion matrix in the notebook - redwood, fir, pine, and birch are all quite distinctive and easy to recognise, but the NN struggles for oak, larch, pine, and poplar. The NN almost completley accuratley predicts poplars as poplars but it also consistently mislabels oaks and larches as poplars aswell. Looking at photos of these trees it can be quite easy to see why, these have quite similar bark strucutres, whereas something like the redwood is very distinctive in texture as well as colour.



Oak Example             |  Poplar Example
:-------------------------:|:-------------------------:
<img src="oak_example.jpg" width="250">  |  <img src="poplar_example.jpg" width="250">

As you can see the oak and poplar have very similar bark patterns, with the main difference being the thickness and protrusion of the lines on the poplar bark

Pine Example          |  Larch Example
:-------------------------:|:-------------------------:
<img src="scots_pine_example.jpg" width="250">  |  <img src="larch_example.jpg" width="250">

Same again here they have very similar bark patterns with the pine having more "stuck on" strips whereas it looks like the larch bark strips are peeling off since each one is a bit convex

After comparing these images it is very easy to see why the NN tripped up on these tree types. Compared to the very distinct other barks below, especially the colour and the "furiness" of the Coastal Redwood:

Douglas Fir Example          |  Coastal Redwood Example   |  Silver Birch Example
:-------------------------:|:-------------------------:|:-------------------------:
<img src="douglas_fir_example.jpg" width="250">  |  <img src="redwood_example.jpg" width="250"> |  <img src="silver_birch_example.jpg" width="250">

For both the sets of similar trees above they have very different canopies and leaf/needle shapes, which can be a more useful signifier of tree type when combined with the bark structure aswell. Due to this there is a future plan to expand the dataset to one of the canopies and branches and training these images on another NN. The output for both these NNs would then instead be a XXX percentage instead of a label, and then combining the results of the two NNs would give a more accurate result.



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



