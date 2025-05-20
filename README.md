# Energy-Consumption-Forecasting
This project is a Streamlit-based web app that predicts energy consumption using weather parameters like humidity, wind speed, and month. It uses a trained machine learning model, fetches real-time weather data via an API, estimates electricity costs, and allows users to download prediction reports.

---

##  Features

- ➤ Predict energy consumption using a trained machine learning model  
- ➤ Fetch live humidity and wind speed data via the WeatherAPI  
- ➤ Estimate electricity costs using user-defined rates  
- ➤ Download prediction reports in CSV format  
- ➤ Clean, responsive interface with customized styling  

---

##  Project Structure

```
├── app.py                      # Main Streamlit app
├── energy_model.pkl           # Trained machine learning model
├── model_train.ipynb          # Jupyter notebook used to train the model
├── weather-energy-data-update.csv # Dataset used for training
├── README.md                  # Project documentation
```

---

##  Model Training

The model was trained using a regression algorithm on the following features:
- Month  
- Humidity  
- Wind Speed  

For detailed training steps and preprocessing, refer to `model_train.ipynb`.

---

##  Usage

To run the app:

```bash
python -m streamlit run app.py
```

> **Note:** Save all four essential files (`app.py`, `energy_model.pkl`, `model_train.ipynb`, and `weather-energy-data-update.csv`) in the same folder.

### Streamlit Sidebar Options:
- ➤ Enter a location (optional) to fetch live weather data  
- ➤ Manually set month, humidity, and wind speed  
- ➤ Predict energy usage and estimate electricity cost  
- ➤ Download results as a CSV report  

---

##  Weather API

The app uses **WeatherAPI** to fetch live humidity and wind speed based on the user's location input.

> Replace the placeholder API key in `app.py`:
```python
api_key = "your_api_key_here"
```

---

##  Requirements

Make sure you have the following Python packages installed:

- streamlit  
- pandas  
- scikit-learn  
- requests  

Install them using:

```bash
pip install -r requirements.txt
```

---

##  Contact

For any queries or suggestions, feel free to open an issue or contribute to the project.

---
