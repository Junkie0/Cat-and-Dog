# Dog and Cat Classification

This project involves building a Convolutional Neural Network (CNN) to classify images of dogs and cats. The dataset used for training and testing the model is available in the "PetImages" directory, containing separate folders for "Cat" and "Dog" images.

## Project Structure

- **/content/PetImages**: Original dataset containing images of cats and dogs.
- **/content/train**: Training dataset after splitting.
- **/content/test**: Testing dataset after splitting.
- **dog_cat_classification.h5**: Saved model file.

## Data Splitting

The dataset is split into training and testing sets using the `train_test_split` function from scikit-learn. Images are moved to their respective directories in the "train" and "test" folders.

## Data Preprocessing

Images are preprocessed using the TensorFlow ImageDataGenerator. The images are scaled to a range of [0, 1] and resized to (224, 224) pixels.

## Model Architecture

The CNN model is built using TensorFlow and Keras. The architecture includes convolutional layers, max-pooling layers, and a dense layer with sigmoid activation for binary classification.

## Model Training

The model is trained using the training dataset and validated on the testing dataset. Training progress, including loss and accuracy, is visualized using matplotlib.

## Model Evaluation

The trained model is evaluated on a sample video dataset containing videos of dogs and cats. The predictions are displayed on the video frames, indicating whether the detected object is a dog or a cat.

## How to Use

1. Clone the repository:

   ```bash
   git clone https://github.com/Junkie0/Cat-and-Dog.git
