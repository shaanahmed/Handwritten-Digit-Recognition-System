### Handwritten Digit Recognition System Using MNIST Dataset (Keras)

#### Overview:
The Handwritten Digit Recognition System is a deep learning project designed to recognize digits (0-9) from handwritten images. The system is built using the MNIST dataset, a collection of 70,000 grayscale images of handwritten digits, each of size 28x28 pixels. The model is trained using Keras, a high-level deep learning API, with TensorFlow as the backend, and employs a deep learning architecture, specifically an Artificial Neural Network (ANN), to perform the classification task.

#### Packages Used:
1. **pyngrok (v4.1.1)**: 
   - Enables exposing the local server to the internet, helpful for sharing a Streamlit app running locally.
  
2. **streamlit-drawable-canvas**: 
   - A Streamlit component allowing users to draw handwritten digits on a canvas in real-time for testing the trained model.
  
3. **streamlit**: 
   - A framework used to build the web interface of the digit recognition system where users can interact and test the system by uploading images or drawing digits.

4. **tensorflow**: 
   - The main deep learning library that provides Keras. Used to build and train the ANN model for digit recognition.
  
5. **opencv-python-headless (v4.5.3.56)**: 
   - A computer vision library used for preprocessing input images, such as resizing or normalizing image data.
  
6. **numpy**: 
   - A fundamental package for array manipulation and numerical operations, used to process and manipulate data in the model.

#### Model Architecture:
- **Input Layer**: Accepts 28x28 pixel images, flattened into a 1D vector of 784 features.
- **Hidden Layers**: One or more dense layers (fully connected layers) with activation functions like ReLU.
- **Output Layer**: A softmax layer with 10 neurons, each representing one of the 10 digits (0-9).
  
#### Training:
The ANN is trained using the MNIST dataset in Keras, where the pixel values are normalized, and categorical crossentropy is used as the loss function. The Adam optimizer is typically used for efficient training, and accuracy is measured to evaluate performance.

#### Streamlit Integration:
- The system integrates with **Streamlit**, allowing users to draw digits in a web interface using **streamlit-drawable-canvas**.
- The drawn digit or uploaded image is preprocessed using **OpenCV** and **NumPy** before being passed to the trained model for prediction.

#### Summary:
This project leverages deep learning techniques using Keras and TensorFlow to recognize handwritten digits, integrating user-friendly features with Streamlit for real-time interaction.
