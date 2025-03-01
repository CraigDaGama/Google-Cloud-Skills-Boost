## **Simple Linear Regression with TensorFlow**

### 📌 **Overview**
This repository contains a basic **TensorFlow** model that learns a simple linear relationship using **supervised learning**. The model is trained using **Stochastic Gradient Descent (SGD)** and Mean Squared Error (MSE) loss.

### 🔧 **Features**
- Uses **TensorFlow** and **NumPy** for training a simple neural network.  
- Logs predictions to **Google Cloud Logging**.  
- Trains on a dataset with a clear linear relationship.  
- Makes predictions after training.

### 🚀 **Installation**
1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/your-repo-name.git
   cd your-repo-name
   ```
2. Install dependencies:
   ```bash
   pip install tensorflow numpy google-cloud-logging
   ```

### 🏃‍♂️ **Usage**
Run the script to train the model and log predictions:
```bash
python model.py
```

### 📖 **How It Works**
- The model is trained on this dataset:
  ```
  xs = [-1, 0, 1, 2, 3, 4]
  ys = [-2, 1, 4, 7, 10, 13]
  ```
- The model learns the relationship and predicts values, e.g., for `x = 10`.

### 📊 **Example Output**
After training, the model predicts:
```
Prediction for 10.0: [Some Value]
```
(Exact value may vary slightly.)

---

