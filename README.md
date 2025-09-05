# Air-Pollution-Forecasting-using-RNN
My 2nd Year Project 




---

# 🌍 Air Pollution Analysis & Prediction

This project analyzes **air pollution data** across major Indian cities and predicts future pollution levels using **LSTM (RNN)**. It also provides **visual insights** and sends **SMS alerts** via Twilio when pollution exceeds safe thresholds.

---


## 🚀 Features

* 📊 **Data Cleaning & Preprocessing** – Handles missing values, extracts time features.
* 📈 **Visualization** – Trend analysis by **year, month, week, and hour** for selected cities.
* 🤖 **Prediction Model** – LSTM-based RNN predicts pollution levels.
* 🔔 **Alert System** – Sends SMS alerts via Twilio if predicted levels exceed thresholds.

---

## 🛠️ Requirements

Install dependencies before running the project:

```bash
pip install -r requirements.txt
```

### requirements.txt

```txt
pandas
matplotlib
seaborn
numpy
tensorflow
scikit-learn
twilio
```

---

## 📊 Dataset

* **File**: `air_quality_data1.csv`
* **Columns include**:

  * `date` (datetime)
  * `city` (city name)
  * `pollution_level`, `CO`, `SO2`, `NOx`, `O3` (pollutants)

---

## ▶️ How to Run the Project

1. **Clone the repository**

```bash
git clone https://github.com/your-username/air-pollution-analysis.git
cd air-pollution-analysis
```

2. **Place the dataset**
   Ensure `air_quality_data1.csv` is in the same folder as `air_pollution_copy.py`.

3. **Run the script**

```bash
python air_pollution_copy.py
```

4. **Outputs you’ll see**:

   * Trend plots for cities (`Mumbai`, `Delhi`, `Kolkata`, `Chennai`).
   * Predicted pollution levels for next year & next 4 months.
   * SMS alert if pollution exceeds threshold.

---

## 📧 SMS Alerts (Twilio Setup)

1. Create a **Twilio account** → [https://www.twilio.com](https://www.twilio.com)
2. Get your **Account SID**, **Auth Token**, and **Twilio phone number**.
3. Replace them inside the script:

```python
account_sid = "your_account_sid"
auth_token = "your_auth_token"
from_ = "+1XXXXXXXXXX"   # Twilio number
to = "+91XXXXXXXXXX"     # Recipient number
```

---

## 📈 Example Output

* **Console Output**

```
Predicted average pollution level in Delhi for next year: 92.15
Predicted pollution levels in Delhi for the next 4 months: [88.23 90.45 91.12 92.78]
Alert sent to Delhi corporation.
```

* **Plots**:

  * Yearly pollution trends
  * Monthly trends
  * Weekly comparisons
  * Hourly variations

---

## 📌 Future Improvements

* Expand dataset with **more cities** and pollutants.
* Deploy prediction model as a **web app (Flask/Streamlit)**.
* Integrate **real-time IoT sensor data**.

---


