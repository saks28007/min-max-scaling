# EXP 4 : Min-Max Scaling.
This repository provides code and results for Min-Max Scaling in data preprocessing. It covers dataset normalization to enhance model performance and interpretability. The project includes examples, visualizations, and comparisons with other scaling techniques, along with best practices and common pitfalls for effective real-world application.

# Experiment Overview
# Steps:
**1. Import required libraries :** *Load the necessary libraries for performing Min-Max Scaling and handling numerical data.*
<br>
**2. Create a NumPy Array (Dataset) :** *Define a numerical dataset as a 2D array, ensuring compatibility with scaling techniques.*
<br>
**3. Initialize MinMaxScaler with Feature Range (0,1) :** *Initialize a scaler that transforms data by mapping its values within a specified range, typically enhancing consistency for machine learning models.*
<br>
**4. Apply Min-Max Scaling to the Data :** *Scale the dataset by normalizing each value based on the minimum and maximum values, ensuring all data points fall within the specified range.*
<br>
**5. Print the Scaled Data :** *Output the transformed dataset, displaying the normalized values after applying Min-Max Scaling.*

# Key Concepts Applied:
**-Importing Libraries :** _Bring in the necessary tools for scaling and handling numerical data._
<br>
**-Creating a Dataset :** _Define a simple numerical dataset in the form of a 2D array._
<br>
**-Initializing the Scaler :** _Prepare a scaling tool to transform data within a chosen range (default: 0 to 1)._
<br>
**-Applying Scaling :** _Adjust all values based on the dataset’s minimum and maximum, fitting them into the specified range._
<br>
**-Normalization Formula :** _Use the formula to rescale each value._
<br>
**-Displaying the results :** _Print the scaled data, now transformed within the defined range._

# Action Plan
**1. Get started with Google Colab :**

 *~Launch Google Colab.*
 <br>
 *~Start a fresh notebook.*

**2. Set Up the Environment :**

*~Ensure that scikit-learn and numpy are installed in your Python environment.*

**3. Import necessary libraries :**

*~Initialize the necessary libraries for the analysis.*
```
from sklearn.preprocessing import MinMaxScaler
import numpy as np
```

**4. Create a Dataset :**

*~Define a numerical dataset as a 2D NumPy array to ensure compatibility with the scaler.*
```
data= np.array([[100],[200],[300],[400],[500]])
```

**5. Initialize Min-Max Scaler :**

*~Set up the scaler to adjust values within a chosen range, typically from 0 to 1.*
```
scalar= MinMaxScaler(feature_range=(0,1))
```

**6. Scale the data :**

*~Apply Min-Max Scaling to normalize the dataset within the chosen range.*
```
scaled_data=scalar.fit_transform(data)
```

**7. Print the Scaled Data :**

*~Display the transformed values to verify the scaling process.*
```
print(scaled_data)
```


































