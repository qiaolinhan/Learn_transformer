# [Unsupervised learning and fastai](https://medium.com/@dhuynh95/an-introduction-to-unsupervised-learning-with-fastai-a6dbd78eca2b)
> Even though transfer learning has enabled people to (re)train effective models on custom and often small data sets, labels are costly to aquire, e.g. medical labels (wildfire images or videos with other informations).

* try to learn our data without asking the model to classify first. __By training an unsupervised feature extractor, and then train a classfier on top of it.__(Maybe not just a classfier?)  
* No longer try to predict a variable $y$, from a variable $x$. Simply try to learn more about the distribution of $x$ it self. (feature extractor?)  

1.) As a beginer of painting: look at the paintings; try to graspthe essence of this; then repaint and try to see whether got something similar; `If not` try to learn from mistakes. 
    Helps to honed 2 skills:  
    * grasping the essence ofthe paintings: look at the raw of images and then extracting features. __ENCODER__  
    * Recovering the original painting from the abstract representation you extracted with the __Encoder__. __DECODER__  
    <img src="https://miro.medium.com/max/220/1*UXJc3rWGKGPuZSs_KcIltw.png">
