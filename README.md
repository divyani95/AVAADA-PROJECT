# CNN Waste Segregation

A deep learning project to **classify different types of waste** (like plastic, metal, glass, etc.) using a **Convolutional Neural Network (CNN)** built with **TensorFlow**.

## 📂 Project Structure
- **Dataset**: Uploaded as a `.zip` and extracted within the notebook.
- **Categories**: Detected dynamically from folders (e.g., `Plastic`, `Metal`, `Glass`, `Cardboard`, etc.)

## 📊 Steps Implemented
1. **Upload and Extract Dataset**
2. **Load Images and Labels**
3. **Visualize Class Distribution**
4. **Preprocess Data** (Resize images to 128x128 and normalize)
5. **Train-Test Split** (80% training, 20% validation)
6. **Build CNN Model** (using Sequential API)
7. **Train the Model** (with EarlyStopping)
8. **Evaluate the Model** (accuracy, loss plots)
9. **Confusion Matrix** (for detailed performance)

## 🧠 CNN Model Architecture
- Input Layer: 128x128x3 images
- 3 × Convolutional Layers (with MaxPooling)
- Flatten Layer
- Dense Layer (128 units, ReLU)
- Output Layer (Softmax activation for multiclass)

> Optimizer: `Adam`  
> Loss: `sparse_categorical_crossentropy`  
> Metrics: `accuracy`

## 🛠️ Requirements
Install dependencies with:
```bash
pip install tensorflow matplotlib scikit-learn Pillow
```

## 🚀 How to Run
- Open the notebook (`CNN_Waste_Segregation.ipynb`) in **Google Colab** or **Jupyter Notebook**.
- Upload your waste dataset `.zip` when prompted.
- Execute cells sequentially to train and evaluate the model.

## 📈 Sample Results
- **Training Accuracy**: ~95% (varies depending on dataset)
- **Validation Accuracy**: ~90%+
- **Confusion Matrix**: Displayed at the end for category-wise performance.

## 📋 Dataset Notes
- The dataset is expected to be organized as:
  ```
  dataset/
    data/
      Plastic/
      Metal/
      Glass/
      Cardboard/
      ...
  ```
- Each subfolder should contain images belonging to that waste category.
