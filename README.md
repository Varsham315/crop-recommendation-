# Crop Recommendation System

A smart **Crop Recommendation System** built using **Flask** that predicts the most suitable crop for cultivation based on soil and environmental parameters. Additionally, it provides fertilizer suggestions to optimize crop growth.

---

##  Features

1. **Crop Prediction**  
   - Predicts the ideal crop using a machine learning model (`XGBoost`) based on soil nutrient values and environmental conditions:
     - Nitrogen (N)
     - Phosphorus (P)
     - Potassium (K)
     - Temperature
     - Humidity
     - pH value
     - Rainfall

2. **Fertilizer Recommendations**  
   - Suggests fertilizers depending on the soil nutrient deficiency/excess.

3. **Text-to-Speech (TTS) Feature**  
   - Converts recommendations into audio using **gTTS** and **pyttsx3** for better accessibility.

4. **Interactive Dashboard**  
   - Provides crop information and fertilizer suggestions via an interactive web interface.

---

## 📦 Technologies Used

- **Backend:** Python, Flask  
- **Machine Learning:** XGBoost (pre-trained model stored as `mainmodel3.pkl`)  
- **Data Handling:** Pandas  
- **Text-to-Speech:** pyttsx3, gTTS  
- **Frontend:** HTML, CSS, Bootstrap  
- **CSV Data:** Fertilizer requirements stored in `fertilizer.csv`  

---

## 🛠️ Installation & Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/croprecommendation.git
   cd croprecommendation

2. **Create a virtual environment:**

   ```bash
   python3 -m venv venv
   source venv/bin/activate   # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies:**

   ```bash
   pip install -r requirements.txt
   ```

4. **Run the application:**

   ```bash
   python app.py
   ```

5. **Open in browser:**

   ```
   http://localhost:5001
   ```

---

## 🧠 How It Works

1. User inputs soil and environmental parameters on the form.
2. The backend processes the inputs and passes them to the pre-trained XGBoost model.
3. The model predicts the most suitable crop.
4. Fertilizer recommendations are calculated based on the difference between actual and required NPK values.
5. The recommendation is displayed on a web page and can be converted to audio using TTS.

---

##  Usage

1. Navigate to **Predict** page.
2. Enter soil nutrient values and environmental parameters.
3. Click **Submit** to view:

   * Recommended crop
   * Fertilizer suggestions
4. Optionally, generate audio of the recommendation using the **Speak** feature.

---

## 🔧 Dependencies

* Flask
* Pandas
* Pickle
* pyttsx3
* gTTS
* XGBoost
* MarkupSafe

Install all dependencies with:

```bash
pip install -r requirements.txt
```

---

## Supported Crops

* Rice, Maize, Chickpea, Kidney Beans, Pigeon Peas, Moth Beans, Mung Bean, Black Gram, Lentil,
* Pomegranate, Banana, Mango, Grapes, Watermelon, Muskmelon, Apple, Orange, Papaya, Coconut, Cotton, Jute, Coffee

---

##  Future Enhancements

* Integrate real-time weather API for dynamic predictions.
* Include regional soil data for more accurate recommendations.
* Mobile-friendly interface with React or Flutter.
* Save user recommendations history with login authentication.

This project is **open-source** and free to use under the [MIT License](LICENSE).

GitHub: [https://github.com/Varsham315](https://github.com/Varsham315)
