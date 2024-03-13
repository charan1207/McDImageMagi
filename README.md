# McDImageRecognition

# Description
McDImageRecognition is a machine learning project focused on image classification for McDonald's fast food items, including Big Mac burgers, French fries, and nuggets. The project   utilizes a Support Vector Machine (SVM) model trained on a dataset of delicious fast food images. A Streamlit web application allows users to upload an image, and the trained model   predicts the category of the McDonald's item, providing a delightful and interactive experience for fast food enthusiasts. Explore the code for a hands-on understanding of image classification in the context of everyone's favorite golden arches.

## Technologies Used:
- **Python:** The primary programming language for the project.
- **scikit-learn:** Utilized for building and training the machine learning model. GridSearchCV is employed for hyperparameter tuning, optimizing SVM parameters (C and gamma).
- **Bing Image Downloader:** A Python library used to download images from Bing for creating the dataset.
- **streamlit:** A web application framework for creating interactive and user-friendly interfaces. The Streamlit app allows users to upload an image and receive predictions from the trained model.
- **numpy and matplotlib:** Used for array operations, data manipulation, and visualization.
- **PIL (Pillow):** Employed for handling image files and facilitating image-related operations.
- **pickle:** Used to serialize and deserialize the trained SVM model for easy storage and retrieval.

## Model Details:
- **Support Vector Machine (SVM):** SVM is a powerful supervised learning algorithm used for classification and regression tasks. In this project, an SVM classifier is employed for image classification.
- **Radial Basis Function (RBF) Kernel:** The RBF kernel is selected for its ability to handle non-linear relationships in the data, making it well-suited for image classification tasks.


## Steps:
1. **Data Collection:**
   In this step, images are collected from Bing using the Bing Image Downloader library. The search terms used for image retrieval are 'pretty sunflower,' 'ruby ball leather,' and 'Ice cream cone.' The images are downloaded and stored 
   in the 'images' directory.
   
   ![image](https://github.com/charan1207/Image_Classification_using_machine_learning/assets/28255223/cb3e4c48-47da-4254-9e37-2131b7f3ba83)

3. **Preprocessing:**
   The collected images undergo preprocessing to make them suitable for model training. Each image is resized to a common size of 150x150 pixels with three color channels (RGB). Additionally, the images are flattened to create a one-dimensional array for each image.

   ![image](https://github.com/charan1207/Image_Classification_using_machine_learning/assets/28255223/aab59863-d65e-4288-9902-f550ade35dba)

   

5. **Model Training:**
   A Support Vector Machine (SVM) classifier is employed for the image classification task. The scikit-learn library is used for implementing the SVM model. Hyperparameter tuning is performed using GridSearchCV to find the optimal     
   values for the regularization parameter (C) and the kernel coefficient (gamma).
  ![image](https://github.com/charan1207/Image_Classification_using_machine_learning/assets/28255223/6c304389-62c2-47ff-99fc-9245f4eb8426)


   
7. **Model Evaluation:**
   The trained model's performance is evaluated using a test set that was previously separated from the dataset. The accuracy score is calculated, and a confusion matrix is generated to assess the model's ability to correctly classify 
   images into the specified categories.
   ![image](https://github.com/charan1207/Image_Classification_using_machine_learning/assets/28255223/269879ce-04f0-405a-a108-0f11f11f5373)

9. **Model Deployment:**
    The trained SVM model is saved for future use using the pickle library. This serialized model can be easily loaded and used to make predictions on new, unseen images without the need to retrain the model.
   
   ![image](https://github.com/charan1207/Image_Classification_using_machine_learning/assets/28255223/06121563-fe7b-4eeb-ae71-9264d8005d76)
10. **Streamlit Web App:**
    A user-friendly web application is developed using Streamlit. Users can interact with the application by uploading an image through the web interface. The uploaded image is then fed into the trained SVM model, and predictions with 
    probabilities for each class are displayed to the user.
    ![image](https://github.com/charan1207/Image_Classification_using_machine_learning/assets/28255223/51bd0684-13ca-4255-a7e8-fd5cf6b15797)




