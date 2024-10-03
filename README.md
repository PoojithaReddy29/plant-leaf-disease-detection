Introduction:

Getting affected by a disease is very common in plants due to various factors such as fertilizers, cultural practices followed, environmental conditions, etc. 
These diseases hurt agricultural yield and eventually the economy based on it.
Any technique or method to overcome this problem and getting a warning before the plants are 
infected would aid farmers to efficiently cultivate crops or plants, both qualitatively and quantitatively. 
Thus, disease detection in plants plays a very important role in agriculture.

Steps:

1. Download Dataset:
First, I downloaded the PlantVillage dataset from Google Drive by using the unique id it holds and unzip the downloaded PlantVillage.zip 
into the PlantVillage dataset folder.

2. Import Libraries:
Importing necessary libraries and modules required to build the classification model.

3. Load Dataset:
Initializing a few parameters required for the image dataset preprocessing.
I used the function convert_image_to_array to resize an image to the size DEFAULT_IMAGE_SIZE.
I loaded the training data images by traversing through all the folders and converting all the images and labels into separate lists respectively.
I examined the labels/classes in the training dataset.

NOTE: I used a small portion of the entire dataset due to the computing limitations. Tweak N_IMAGES to include entire dataset.

4. Augment and Split Dataset:
Using ImageDataGenerator to augment data by performing various operations on the training images.
Splitting the data into training and test sets for validation purpose.

5. Build Model:
Defining the hyperparameters of the plant disease classification model.

6. Train Model:
I initialized Adam optimizer with learning rate and decay parameters.
I choose the type of loss and metrics for the model and compiled it for training.

7. Evaluate Model:
Comparing the accuracy and loss by plotting the graph for training and validation.

8. Save Model
   
9. Test Model:
The predict_disease function to predict the class or disease of a plant image.
We just need to provide the complete path to the image and it displays the image along with its prediction class or plant disease.

10. Reuse Model:
We download the trained model and label transform saved in the Google Drive.


