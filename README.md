
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
 
</head>
<body>

  <h1>📍 Earthquake Prediction</h1>
  <p>
   The Earthquake Magnitude Prediction project focuses on predicting earthquake magnitudes using regression models while visualizing geographical earthquake distributions through interactive maps. The dataset comprises historical earthquake records with features such as latitude, longitude, date, time, and magnitude, alongside additional characteristics. Data preprocessing involved creating a unified timestamp column, normalizing features, encoding categorical variables, and splitting the dataset for training and testing. The models employed include Ridge Regression for linear predictions with regularization, Decision Tree Regressor for capturing non-linear patterns, and K-Nearest Neighbors (KNN) Regressor for distance-based predictions. Metrics such as accuracy, mean absolute error, mean squared error, and execution time were evaluated for performance comparison. Visualizations include scatter plots for actual vs. predicted values, bar charts for model performance, and an interactive map using `folium` to display earthquake locations with clustering. The project utilized libraries like `numpy`, `pandas`, `sklearn`, `matplotlib`, and `folium`. Future work involves integrating additional features, testing advanced models like Random Forest or XGBoost, and automating real-time earthquake data integration to enhance prediction accuracy and insights.
  </p>

  <h2>📌 Key Objectives</h2>
  <ul>
    <li>Visualize earthquake locations using <code>folium</code> with clustering</li>
    <li>Enable real-time coordinate updates via widgets</li>
    <li>Train ML regression models on earthquake data to predict magnitudes</li>
    <li>Compare model accuracies and performance</li>
  </ul>

  <h2>🗺️ Interactive Mapping with Folium</h2>
  <ul>
    <li>CSV with latitude and longitude columns is loaded using <code>pandas</code></li>
    <li>Markers for all earthquake points are plotted using <code>MarkerCluster</code></li>
    <li>Users can input coordinates to dynamically update and center the map using <code>ipywidgets</code></li>
  </ul>

  <h3>💡 Features:</h3>
  <ul>
    <li>Map updates on user input via widgets</li>
    <li>Markers show location index with pop-up</li>
    <li>Exportable HTML map using <code>folium.Map().save()</code></li>
  </ul>

  <h2>🧠 Machine Learning Models</h2>

  <h3>1. Ridge Regression</h3>
  <ul>
    <li>Accuracy: <code>62.77%</code></li>
    <li>MAE: <code>0.059</code>, RMSE: <code>0.080</code></li>
  </ul>

  <h3>2. Decision Tree Regressor</h3>
  <ul>
    <li>Accuracy: <code>99.18%</code> — highest accuracy among tested models</li>
    <li>Well-suited for non-linear patterns in geographic/magnitude data</li>
  </ul>

  <h3>3. K-Nearest Neighbors (KNN) Regressor</h3>
  <ul>
    <li>Initial accuracy for k=6: <code>78.89%</code></li>
    <li>Model evaluated for multiple k values from 2–10</li>
    <li>Execution time and accuracy plotted for various k values</li>
  </ul>

  <h3>📊 Accuracy vs k (KNN)</h3>
  <pre>
For k = 6 : Accuracy = 0.7889908031677613
For k = 7 : Accuracy = 0.7839443025845729
For k = 10 : Accuracy = 0.7690226861643044
For k = 8 : Accuracy = 0.7792516079528771
For k = 4 : Accuracy = 0.7986960127931608
For k = 5 : Accuracy = 0.7939315396816573
For k = 3 : Accuracy = 0.8011112421148958

  </pre>

 
  <h2>📉 Accuracy Comparison Across Models</h2>
<p>This chart compares the test accuracy of all three models. It helps in identifying the most reliable regression method for earthquake data:</p>

<!-- Replace with your actual image path or name -->
<img src="accuracy_comparison.png" alt="Accuracy Comparison Chart" style="max-width: 100%; border: 1px solid #ccc; padding: 6px; background: #fff;">

  <h2>✅ Conclusion</h2>
  <ul>
    <li><strong>Decision Tree</strong> offers the highest accuracy and is best suited for this dataset</li>
    <li><strong>Folium</strong> provides powerful geospatial interactivity for visualizing earthquakes</li>
    <li>Widgets allow easy exploration of earthquake coordinates and locations</li>
    <li>KNN is tunable and provides moderate performance with quick prototyping</li>
  </ul>

  <h2>🔮 Future Work</h2>
  <ul>
    <li>Integrate real-time earthquake API like USGS or EMSC</li>
    <li>Include temporal analysis (time series forecasting of aftershocks)</li>
    <li>Deploy as a web app using Streamlit or Flask</li>
    <li>Add magnitude-based color scaling on map markers</li>
  </ul>

  <h2>📁 Files Generated</h2>
  <ul>
    <li><code>earthquake_map.html</code> – Interactive map with all plotted points</li>
    <li><code>model_accuracy_plot.png</code> – Accuracy vs. K graph</li>
    <li><code>execution_time_plot.png</code> – Execution time vs. K</li>
  </ul>

  <h2>📬 Contact</h2>
  <p>
    For queries, feedback, or collaboration: <a href="mailto:kesavardhan775@gmail.com">your.email@example.com</a><br>
    GitHub: <a href="https://github.com/keshav-077">https://github.com/your-profile</a>
  </p>

</body>
</html>
