# Plant-Disease-Detection
The goal of this Repo is to utilize Deepl learning to categorize photos from the PlantVillage Dataset. There are thousands of photos in the PlantVillage collection, which includes 38 categories of plants. 
this dataset contains images of plants belonging to 38 different categories. The images were acquired by searching the web and taking pictures.

## About Dataset:
Human society needs to increase food production by an estimated 70% by 2050 to feed an expected population size that is predicted to be over 9 billion people. 
Currently, infectious diseases reduce the potential yield by an average of 40% with many farmers in the developing world experiencing yield losses as high as 100%. 
The widespread distribution of smartphones among crop growers around the world with an expected 5 billion smartphones by 2020 offers the potential of turning the smartphone into a valuable tool for diverse communities growing food. 
One potential application is the development of mobile disease diagnostics through machine learning and crowdsourcing. 
Here we announce the release of over 50,000 expertly curated images on healthy and infected leaves of crops plants through the existing online platform PlantVillage. We describe both the data and the platform. 
These data are the beginning of an on-going, crowdsourcing effort to enable computer vision approaches to help solve the problem of yield losses in crop plants due to infectious diseases.

## Installation Instructions:
- I have provided a Txt file that contains all the libraries that you need to run the notebook the file name is **"requirements.txt"** and also provides **"conda.yaml"** these two files for the final model.
- If you want to use mlflow and see the experiment tracking I did, you can use this command in cmd after activating the environment **"mlflow server --backend-store-uri sqlite:///mlflow.db --default-artifact-root ./artifacts --host 0.0.0.0 --port 5000"** before this you should download the database and the artifacts file.
- just download the dataset from this **[Dataset](https://www.kaggle.com/datasets/abdallahalidev/plantvillage-dataset)** then download the repo and here you are ready to run the code or you can use the model.h5 instead of all the steps.

## Usage Guide:
- I put the image paths and labels from the mat file into a dataframe to make it easier for me here is the snippet
  
 ![dataframe](https://github.com/Bassem-2000/Images/blob/main/dataframe.png?raw=true)
 
- after that, I used ImageDataGenerator from keras to load the data by applying some data augmentation to the training dataset here is the snippet
  
 ![ImageDataGenerator](https://github.com/Bassem-2000/Images/blob/main/ImageDataGenerator.png?raw=true)

## Model Architecture:
- I used the Resnet Architecture and used different fine-tuning and architecture but my final model and architecture are done by applying fine-tuning to the final layers as I made the last 15 layers nontrainable and add some neurons here is the snippet for the model summary
  
 ![Architecture](https://github.com/Bassem-2000/Images/blob/main/Architecture.png?raw=true)


## Evaluation:
- I used different approaches to test the performance of the architecture and the model like accuracy, loss, Recall and Precision all of these approaches were used on every architecture I did and you can see it from the mlflow experiment tracking you can download the database and files to test it by yourself, here are the final model performance:
  
 ![Accuracy](https://github.com/Bassem-2000/Images/blob/main/accuracy.png?raw=true)
 ![Loss](https://github.com/Bassem-2000/Images/blob/main/Loss.png?raw=true)
 ![Recall](https://github.com/Bassem-2000/Images/blob/main/Recall.png?raw=true)
 ![Precision](https://github.com/Bassem-2000/Images/blob/main/Precision.png?raw=true)

## Example:
- I test the model with a random image and visualize it here you can see the image with the prediction:

 ![Example](https://github.com/Bassem-2000/Images/blob/main/Example.png?raw=true)


## Contact:

[<img alt="alt_text" width="30px" src="https://cdn2.iconfinder.com/data/icons/social-media-2285/512/1_Whatsapp2_colored_svg-512.png" />](https://wa.me/+201006491306)
&nbsp;&nbsp;
[<img alt="alt_text" width="30px" src="https://cdn2.iconfinder.com/data/icons/social-media-2285/512/1_Linkedin_unofficial_colored_svg-512.png" />](https://www.linkedin.com/in/bassem-ahmed-ahmed/)
&nbsp;&nbsp;
[<img alt="alt_text" width="30px" src="https://cdn4.iconfinder.com/data/icons/social-media-logos-6/512/112-gmail_email_mail-256.png" />](mailto:bassemahmed.am@gmail.com)
&nbsp;&nbsp;
[<img alt="alt_text" width="30px" src="https://cdn2.iconfinder.com/data/icons/social-media-2285/512/1_Facebook2_colored_svg-512.png" />](https://www.facebook.com/bassem.ahmed.7712/)

Can you please provide me with feedback on how I can improve myself and any ideas to improve the model, I am eager to receive any advice that can help me develop my skills.

&nbsp;&nbsp;
**Wish you a nice day :)**
