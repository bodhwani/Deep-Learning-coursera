# Face Recognition
### Verification vs Recognition
>
![alt text](../images/vr.png "vr")


### One Shot Learning
It means you will be given only one shot to recognize that person.
<br>
Feeding images into CNN and using softmax funciton as an output, will not work here.
Two reasons :
- Dataset is very small so it will not be able to predict only with one image during testing.
- Suppose new person came,  then do we need to retrain our model?
This isn't a good approach.Here comes One Shot : Learning similarity function


![alt text](../images/smf.png "smf")


But how to calculate d?
**Lets look at Siamese network**

### Siamese network
>
![alt text](../images/sm.png "sm")


### Triple loss
For this, we need to compare pair of images
<br>
Triple - We will be looking at three images, simaltaneously
- Anchor 
- Positive
- Negative
>
![alt text](../images/tripleloss.png "tripleloss")

>

**Loss Function**
>
![alt text](../images/formulaetl.png "formulaetl")


How will we choose parameters - A,P,N
We can't chose them randomly. 
>
<!-- ![alt text](../images/choosetl.png "choosetl")
 -->

### Binary Classification
Face Verification's another method.
- 1=Same persons
- 2=Different persons


# Neural Style Transfer
What is NST?
>
![alt text](../images/nst.png "nst")

**How better is the generated image?**
Define cost function : J
>
![alt text](../images/nstCF.png "nstCF")

In order to actaullly generate new image, do the following :
>generatedI

There are two things :
- Content cost function
- Style cost function

Overall cost function of NST :
>
![alt text](../images/overallCF.png "overallCF")

The first part is chosen somewhere in the middle, neither to shallow, nor to deep.
### Content Cost function
>
![alt text](../images/ccf.png "ccf")

### Style Cost function
>
![alt text](../images/scf1.png "scf1")

>
![alt text](../images/scf2.png "scf2")



If they are highly correlated, G will be high. Otherwise, it will be small.

Style Matrix :
>
![alt text](../images/smatrix.png "smatrix")


### 1D and 3D generalizations
**1D** :
>
![alt text](../images/1D.png "1D")


**3D:**
>
![alt text](../images/3D.png "3D")


