# PCOS-detection
Polycystic Ovary Syndrome Detection from Ultrasound images using Transfer Learning models


AIM:
	To develop a disease diagnostics for PCOS by classifying images as either depicting individuals diagnosed with polycystic ovary syndrome or not.

DATASET DESCRIPTION:
	 A Datasets included ultrasound pictures of healthy ovaries as well as cystic ovaries.The ultrasound photos that showed infected cysts on the ovary were given the label ‘infected’ while the ultrasound images that showed a healthy ovary were given the label ‘not infected’. 

DATA PREPROCESSING:
	ImageDataGenerator class from the Keras library to perform various preprocessing techniques like rescaling, shear transform, zoom, flip, rotate and fill mode on image data. 

MODEL USED: 
InceptionV3, DenseNet and MobileNet

PROCESS FLOW:

1.Transfer learning was used with the respective models as a starting point.

2. The pre-trained models were loaded without the top layers.

3. Custom top layers were added to adapt the model to the specific dataset.

4. The model was compiled using the Adam optimizer and categorical crossentropy loss.

5. Data generators were utilized to provide the model with augmented data during training.

6. The model was trained for 10 epochs with a batch size of 32 and specific hyperparameters.

7. The validation set was used to determine that accuracy.

	
	
	

MODEL COMPARISON:

MobileNet :    loss: 2.9671 - accuracy: 0.5000

DenseNet :      loss: 0.2136 - accuracy: 0.9222

InceptionV3 :  loss: 0.0041 - accuracy: 0.9988


INFERENCE:

![image](https://user-images.githubusercontent.com/114279270/235894575-beda9e3f-36b9-4ddb-a032-0d43115b0373.png)



