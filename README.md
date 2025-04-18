
<h2><b>Time Series Forecasting for Appliances Energy Prediction</b></h2>
<h3><b>Overview</b></h3>
This project focuses on predicting appliance energy consumption using a multivariate time-series dataset. The dataset records various environmental and temporal features at 10-minute intervals. The goal is to build a deep learning-based supervised model capable of learning patterns and dependencies from these inputs to forecast future energy usage.

<h3><b>Project Details</b></h3>

<h5><b>Introduction</b></h5>
Energy is a vital element for sustainable development and economic growth. Efficient monitoring and forecasting of energy consumption allows better planning, optimization, and management of resources—especially in residential and commercial buildings. This project aims to predict appliance energy consumption using advanced machine learning techniques.

<h5><b>Data Insights</b></h5>
  <ul>
    <li><strong>Hourly Distribution:</strong> Highest electricity consumption occurs between 17:00 and 20:00, while the lowest is observed between 23:00 and 06:00.</li>
    <li><strong>Weekday Distribution:</strong> Electricity consumption on Sundays is significantly higher than on other days.</li>
    <li><strong>General View:</strong> Temperature shows an overall increasing trend, while other features do not show significant patterns.</li>
    <li><strong>Appliances Usage:</strong> Electricity usage does not follow a clear pattern over time, indicating the need for deeper analysis to uncover hidden trends.</li>
  </ul>

  <h5><b>Visualization</b></h5>
  <ul>
    <li><strong>Randomly Selected Weekly Data:</strong> Regular ups and downs in energy use suggest hidden habits or routines in appliance usage.</li>
    <li><strong>Histogram for Appliances:</strong> The data is positively skewed with some high energy use.</li>
  </ul>

  <h5><b>Correlation Analysis</b></h5>
  <ul>
    <li><strong>Strongest Correlations:</strong> Time of day (0.22) and number of lights on (0.20).</li>
    <li><strong>Weak Correlations:</strong> Air pressure (-0.15) and other environmental factors show weak relationships with appliance usage.</li>
  </ul>

  <h5><b>Clustering Analysis</b></h5>
  <ul>
    <li><strong>Temperature-Related Plots:</strong> Show distinct groupings, indicating reliable classification.</li>
    <li><strong>Humidity-Related Plots:</strong> Show less clear separation.</li>
  </ul>

  <h5><b>Preprocessing and Feature Engineering</b></h5>
  <ul>
    <li><strong>No Missing Values:</strong> The dataset is complete.</li>
    <li><strong>Feature Engineering:</strong> Time-based features and feature scaling using MinMaxScaler were applied to normalize values.</li>
  </ul>

  <h5><b>Model Design</b></h5>
  <ul>
    <li><strong>LSTM Model:</strong> An LSTM-based sequential model was used to capture temporal dependencies. The architecture included one LSTM layer with 64 units, a Dropout layer, and a Dense output layer. The model was compiled with Mean Squared Error (MSE) as the loss function.</li>
  </ul>

 <h5><b>Results</b></h5>
  <ul>
    <li><strong>ARIMA and LSTM Models:</strong> Both models showed reasonable performance, with LSTM achieving better accuracy after optimization.</li>
    <li><strong>Optimization Techniques:</strong> Time-based cyclical features and hyperparameter tuning were used to improve model performance.</li>
  </ul>

   <h3><b>Setup Instructions</b></h3>

 <h2>Clone the Repository</h2>
  <pre>
git clone https://github.com/geesarani/Appliance_Energy_Prediction-.git
cd Appliance_Energy_Prediction-
  </pre>

  <h2>Install Dependencies</h2>
  <pre>
pip install -r requirements.txt
  </pre>

  <h2>Run the Jupyter Notebook</h2>
  <pre>
cd notebooks
jupyter notebook Appliance_Energy_Prediction.ipynb
  </pre>


  <h4><b>Data Preprocessing</b></h4>
  <p>The preprocessing steps are included in the <code>EDA.ipynb</code> notebook. Run the cells to clean and preprocess the data.</p>

  <h4><b>Feature Engineering</b></h4>
  <p>Feature engineering steps are included in the <code>Appliance_Energy_Prediction.ipynb</code> notebook. Run the cells to create new features and prepare the data for modeling.</p>

  <h4><b>Model Training</b></h4>
  <p>The model training code is also in the <code>Appliance_Energy_Prediction.ipynb</code> notebook. Run the cells to train the ARIMA and LSTM models.</p>

  <h4><b>Model Evaluation</b></h4>
  <p>Evaluate the models using the provided metrics (RMSE, MAE, etc.) and visualize the results.</p>

  <h4><b>Optimization</b></h4>
  <p>Hyperparameter tuning and optimization techniques are included in the notebook. Run the cells to optimize the model parameters.</p>



