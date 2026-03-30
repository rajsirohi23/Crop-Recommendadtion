## Crop Recommendation Web App

Simple Flask web application that loads a pre-trained Random Forest model from `crop_reco_model.pkl` and suggests a suitable crop based on user-provided soil and weather conditions.

### Assumed model inputs

This app assumes the model expects the following 7 numeric features in this exact order (1 row per prediction):

1. `N` – Nitrogen
2. `P` – Phosphorus
3. `K` – Potassium
4. `temperature` – Temperature in °C
5. `humidity` – Relative humidity in %
6. `ph` – Soil pH
7. `rainfall` – Rainfall in mm

If your model uses a different feature set or ordering, adjust the `feature_names` list and form fields accordingly in `app.py` and `templates/index.html`.

### Setup

1. **Create and activate a virtual environment (recommended)**

   ```bash
   cd "/Users/rajsirohi/Desktop/Crop recomm"
   python3 -m venv .venv
   source .venv/bin/activate  # On Windows: .venv\Scripts\activate
   ```

2. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

3. **Run the Flask app**

   ```bash
   python app.py
   ```

4. **Open in browser**

   Visit `http://127.0.0.1:5000/` in your browser and enter the input values to get a crop recommendation.

### Notes

- The model is loaded from `crop_reco_model.pkl` in the project root when the app starts.
- The `/predict` endpoint accepts both normal HTML form submissions and JSON requests. For programmatic use, you can send a `POST` request with JSON containing the 7 fields listed above.

