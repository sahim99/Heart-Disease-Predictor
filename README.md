prediction = model.predict(input_data_reshaped)

# ❤️ Heart Disease Predictor

Welcome! This project helps you predict the risk of heart disease using real patient data and machine learning. It's designed to be simple, practical, and easy to use—even if you're new to data science.

## 🚀 What Does This Project Do?

- Loads and explores heart disease data from a CSV file
- Splits the data into training and test sets for fair evaluation
- Trains a logistic regression model to make predictions
- Shows you how accurate the model is
- Lets you test new patient data to see the prediction in action

## 🧠 How It Works

1. **Import the essentials**: numpy, pandas, and scikit-learn
2. **Load your data**: Just make sure `heart_disease_data.csv` is in the project folder
3. **Prepare the data**: Separate features (`x`) and target labels (`y`)
4. **Split for training and testing**: So you know how well your model performs
5. **Train the model**: Logistic regression is simple and effective for this task
6. **Check accuracy**: See how well it predicts on both training and test data
7. **Make predictions**: Try out new patient data and get instant results

## 🛠️ How to Use

1. **Clone this repo**
   ```sh
   git clone https://github.com/sahim99/Heart-Disease-Predictor.git
   cd Heart-Disease-Predictor
   ```
2. **Install the required packages** (it's best to use a virtual environment):
   ```sh
   pip install -r requirements.txt
   ```
3. **Open and run the notebook**
   - Use Jupyter Notebook or VS Code to open `Heart-Disease-Prediction-code.ipynb`
   - Step through the cells to see each part in action

## 📊 Data

Make sure your dataset is named `heart_disease_data.csv` and placed in the root directory of the project.

## 🩺 Example: Predicting Heart Disease

Here's how you can use the model to predict heart disease for a new patient:

```python
input_data = (63,1,3,145,233,1,0,150,0,2.3,0,0,1)
input_data_as_numpy_array = np.asarray(input_data)
input_data_reshaped = input_data_as_numpy_array.reshape(1,-1)
prediction = model.predict(input_data_reshaped)
if prediction[0] == 0:
    print("The Person does not have Heart Disease")
else:
    print("The Person has Heart Disease")
```

## 📦 Requirements

- Python 3.11 or newer
- numpy
- pandas
- scikit-learn

## 📄 License

This project is open source and available under the MIT License. Feel free to use, modify, and share!
