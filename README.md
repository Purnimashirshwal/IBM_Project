📌 Project Description
This is a deep learning project to classify animal images. It automatically detects whether the image contains a cat or a dog using a trained CNN model. The model learns from thousands of example images and gives accurate results on new unseen images.

🎯 Objective
To create an AI model that can classify any given pet image as either a cat or a dog with high accuracy.

🛠️ Technologies Used
- Python – The main language used for development.
- TensorFlow & Keras – Used to build and train the CNN model easily.
- NumPy – For working with arrays and numerical data (like image pixels).
- Matplotlib – For plotting accuracy and loss graphs.
- Google Colab – Free online platform with GPU support for training the model faster.
- 
📁 Dataset
- Dataset Name: cats_and_dogs_filtered
- Source: TensorFlow Datasets
- Size: 2000+ labeled images (Cats and Dogs)
- Split: Already split into training and validation folders
  
🧠 Model Architecture
Input Layer (150x150x3)
→ Conv2D + ReLU
→ MaxPooling2D
→ Conv2D + ReLU
→ MaxPooling2D
→ Conv2D + ReLU
→ MaxPooling2D
→ Flatten
→ Dense (512)
→ Dense (1) with Sigmoid activation

🚀 How I Made This Project
1. Loaded the dataset using TensorFlow’s utilities.
2. Resized all images to 150x150 pixels.
3. Normalized pixel values between 0 and 1.
4. Created a CNN model using Keras Sequential API.
5. Trained the model for 20 epochs with batch size of 32.
6. Evaluated the model using validation accuracy and plotted performance graphs.
   
📊 Results
-The model reached over 91% accuracy on validation data.
-Training and validation accuracy both improved over time. Loss decreased consistently, showing the model was learning effectively.

🚧 Challenges Faced
- Limited Data: Only 2000+ images, so had to be careful with overfitting.
- Model Tuning: Needed to experiment with layers and activation functions.
- Preprocessing Consistency: All images needed to be resized and normalized exactly the same.
- Training Time: Without GPU, training would’ve been very slow — used Google Colab for speed.
  
🔮 Future Scope
- Use more diverse and larger datasets for improved generalization.
- Train model to classify more than just cats and dogs (multi-class).
- Deploy as a web or mobile app using Streamlit or TensorFlow Lite.
- Add real-time camera integration for live pet detection.

