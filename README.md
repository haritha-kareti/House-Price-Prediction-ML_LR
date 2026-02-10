<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>House Price Prediction using MLR</title>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <!-- Bootstrap CDN -->
    <link rel="stylesheet"
          href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">

    <style>
        body {
            background-color: #f4f6f9;
            font-family: "Segoe UI", sans-serif;
            line-height: 1.7;
        }
        .container {
            background: #ffffff;
            padding: 30px;
            margin-top: 40px;
            margin-bottom: 40px;
            border-radius: 10px;
            box-shadow: 0px 4px 15px rgba(0,0,0,0.1);
        }
        h1, h2 {
            color: #2c3e50;
            margin-top: 30px;
        }
        h1 {
            text-align: center;
            margin-bottom: 20px;
        }
        ul li {
            margin-bottom: 8px;
        }
        code {
            background: #eef1f5;
            padding: 3px 6px;
            border-radius: 5px;
        }
        footer {
            text-align: center;
            margin-top: 40px;
            color: #777;
        }
        a {
            color: #007bff;
        }
    </style>
</head>

<body>

<div class="container">

    <h1>🏠 House Price Prediction Using Multiple Linear Regression</h1>

    <h2>📘 Introduction</h2>
    <p>
        Predicting house prices is an important application of Machine Learning in the real estate industry.
        This project uses a <strong>Multiple Linear Regression (MLR)</strong> model implemented in Python to
        estimate house prices based on various features such as location, size, number of bedrooms, and year built.
        The model follows an object-oriented approach and includes training, testing, evaluation, and model persistence.
    </p>

    <h2>🎯 Objectives</h2>
    <ul>
        <li>Predict house prices using multiple independent variables</li>
        <li>Evaluate model performance using RMSE and R² score</li>
        <li>Implement training and testing phases</li>
        <li>Save and reload the trained model</li>
        <li>Allow prediction for new house data</li>
    </ul>

    <h2>🧰 Requirements</h2>

    <h5>Software Requirements</h5>
    <ul>
        <li>Python 3.x</li>
        <li>Google Colab / Jupyter Notebook / VS Code</li>
    </ul>

    <h5>Python Libraries</h5>
    <ul>
        <li>NumPy</li>
        <li>Pandas</li>
        <li>Scikit-learn</li>
        <li>Pickle</li>
        <li>Warnings</li>
        <li>Sys</li>
    </ul>

    <h2>📊 Dataset Description</h2>
    <p>
        The dataset is provided in CSV format. The first column represents the target variable
        (<strong>house price</strong>) and the remaining columns represent independent features.
        Categorical variables such as <code>city</code> and <code>country</code> are encoded numerically.
    </p>

    <h2>⚙️ Model Workflow</h2>

    <h5>1️⃣ Data Loading & Preprocessing</h5>
    <ul>
        <li>Dataset loaded using Pandas</li>
        <li>Categorical features converted into numerical values</li>
        <li>Features and target variable separated</li>
        <li>Data split into 80% training and 20% testing</li>
    </ul>

    <h5>2️⃣ Model Training</h5>
    <p>
        A <strong>LinearRegression</strong> model is trained using the training dataset.
        Predictions are generated and stored for performance evaluation.
    </p>

    <h5>3️⃣ Training Loss (RMSE)</h5>
    <p>
        Root Mean Square Error (RMSE) is calculated manually to measure the average prediction error:
    </p>
    <p><code>RMSE = sqrt( Σ(y - ŷ)² / n )</code></p>

    <h5>4️⃣ Training Accuracy (R² Score)</h5>
    <p>
        R² score indicates how well the model explains the variance in house prices.
        A higher value indicates better performance.
    </p>

    <h5>5️⃣ Model Testing</h5>
    <ul>
        <li>Predictions are made on unseen test data</li>
        <li>Test RMSE and Test R² score are calculated</li>
        <li>Helps evaluate model generalization</li>
    </ul>

    <h5>6️⃣ Price Prediction</h5>
    <p>
        The model allows prediction of house price by providing custom input values such as
        bedrooms, bathrooms, square footage, city, and year built.
    </p>

    <h5>7️⃣ Model Saving & Loading</h5>
    <p>
        The trained model is saved using <code>pickle</code> and can be reloaded later without retraining,
        making it suitable for deployment.
    </p>

    <h2>🧠 Key Features</h2>
    <ul>
        <li>Object-Oriented Programming approach</li>
        <li>Manual RMSE and R² calculation</li>
        <li>Train-test split implementation</li>
        <li>Model persistence using pickle</li>
        <li>Extendable for web applications</li>
    </ul>

    <h2>📈 Results</h2>
    <p>
        The model provides training and testing RMSE along with R² accuracy.
        Lower RMSE and higher R² indicate good predictive performance.
    </p>

    <h2>🚀 Future Enhancements</h2>
    <ul>
        <li>Use One-Hot Encoding for categorical features</li>
        <li>Apply feature scaling</li>
        <li>Compare with Ridge, Lasso, and Random Forest models</li>
        <li>Deploy using Flask or Django</li>
        <li>Add visualization dashboards</li>
    </ul>

    <h2>🧾 Conclusion</h2>
    <p>
        This project demonstrates the effective use of Multiple Linear Regression for predicting house prices.
        The model is accurate, modular, and suitable for real-world applications.
        It provides a strong foundation for advanced machine learning and deployment projects.
    </p>

    <h2>🔗 References</h2>
    <ul>
        <li><a href="https://scikit-learn.org/stable/modules/linear_model.html" target="_blank">Scikit-learn Linear Regression</a></li>
        <li><a href="https://pandas.pydata.org/docs/" target="_blank">Pandas Documentation</a></li>
        <li><a href="https://numpy.org/doc/" target="_blank">NumPy Documentation</a></li>
        <li><a href="https://www.geeksforgeeks.org/ml-linear-regression/" target="_blank">Linear Regression – GeeksforGeeks</a></li>
    </ul>

    <footer>
        <p>© 2026 | House Price Prediction using MLR</p>
    </footer>

</div>

</body>
</html>
