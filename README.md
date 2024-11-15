# Astronomy--NeuralNet-Classification
A Neural Network Model
## Summary:
The basis of this project was to practice and exhibit basic creation of a neural network using a dataset about one of my most loved aspirations which is astronomy. The dataset depicts image information about celestial bodies that are either classified as a quasar, star or galaxy. I will do a continuation of this project that will undergo the classification using the images themselves, rather than the data collected on them, and test which one poses a higher AUC Score. What adds complexity to this model is the usage of 3 output classes.

## Depiction of Columns

![image](https://github.com/user-attachments/assets/3f3c4b1f-cef6-4a06-b618-afbba9fa0b6c)


## Data Interpretation
The confusion matrix shows correlation between distinct features. This allows me to discern which features relate most the the models score, and how they interact with eachother.

![image](https://github.com/user-attachments/assets/d59bee05-3443-46e4-8158-80dff9d50e95)


The r vs. i shows a high correlation. This is because r is the red filter displayed in the photometric system, and i is the infared filter in the photometric system.
The matrix also shows a redshift correlation in the quasar class specifically. Redshifts in quasars are measured due to the strong spectral lines in their ultraviolet emmision spectrum. This correlation is very good as it creates a strong connection between redshifts and quasars, which will help the model understand that class better. 

## Techniques
For the model, I built my own neural network which was equally deep than it is wide. Data prep was crucial as the classes needed to be split up using dummies, to give each class a one hot encoded style. This allowed for an easy train test split and a 3 neuron, dense output layer.

![image](https://github.com/user-attachments/assets/638f601c-be22-4de1-b964-fe9abd4ac89e)

![image](https://github.com/user-attachments/assets/e21f260d-ca6f-44a3-b018-38cdeba1c42d)

## Other methods
Using an argmax function allowed me to specifically classify each row and give them a value.

![image](https://github.com/user-attachments/assets/a8eab393-6a5f-4cb5-859a-e6a7fd0dc15e)

## Score
This model boasts a 94% AUC Score. Certain tweaks can be made to troubleshoot a better score, like the depth of the network.

![image](https://github.com/user-attachments/assets/421935bc-5ff2-4300-a25e-661191473529)
