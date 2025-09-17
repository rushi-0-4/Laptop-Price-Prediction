# laptop-price-predictor
---

# 💻 Laptop Price Prediction

This project is a **machine learning web app** that predicts the price of a laptop based on its hardware specifications. It uses a **Linear Regression model** trained on a dataset of laptop specifications and prices.

## 🚀 Features

* Data preprocessing with **Pandas & NumPy**
* Extracts memory types (HDD, SSD, Flash, Hybrid) from raw dataset
* Machine learning with **Scikit-learn** (Linear Regression)
* Model saved using **Pickle**
* Web interface built with **Flask**
* User inputs laptop specs (RAM, HDD, SSD, Flash, Hybrid) → predicts price

## 📂 Project Structure

```
Laptop Price Prediction/
│
├── main.py          # Data preprocessing, model training, save model.pkl
├── server.py        # Flask server for prediction
├── laptop_data.csv  # Dataset
├── model.pkl        # Trained Linear Regression model
├── templates/
│   └── home.html    # Frontend UI for input/output
└── README.md        # Project documentation
```
## 💻 Output Screens


![output photo](https://github.com/Mecsan/laptop-price-predictor/blob/master/output/Screenshot%20(166).png?raw=true)

![output photo](https://github.com/Mecsan/laptop-price-predictor/blob/master/output/Screenshot%20(167).png?raw=true)

## ⚙️ Installation & Setup

1. **Clone the repository**

   ```bash
   git clone https://github.com/rushi-0-4/laptop-price-prediction.git
   cd laptop-price-prediction
   ```

2. **Create a virtual environment (optional but recommended)**

   ```bash
   python -m venv venv
   source venv/bin/activate   # On Mac/Linux
   venv\Scripts\activate      # On Windows
   ```

3. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

   *(If `requirements.txt` not created yet, install manually: `pip install flask numpy pandas scikit-learn`)*

4. **Train the model (if needed)**

   ```bash
   python main.py
   ```

   This will generate `model.pkl`.

5. **Run the Flask app**

   ```bash
   python server.py
   ```

   Open your browser at `http://127.0.0.1:5000/`

---

## 🖥️ Example Input/Output

* Input:

  * RAM: `16 GB`
  * HDD: `512 GB`
  * SSD: `256 GB`
  * Flash: `0 GB`
  * Hybrid: `0 GB`

* Output:

  ```
  Predicted Laptop Price: ₹ 62,450
  ```

---

## 🛠️ Tech Stack

* **Python 3**
* **Flask** (backend & UI)
* **NumPy, Pandas** (data preprocessing)
* **Scikit-learn** (machine learning model)

---

## 📊 Dataset

* Dataset: `laptop_data.csv`
* Features include RAM, Memory type (HDD, SSD, Flash, Hybrid), etc.
* Target: Laptop Price

---

## 📌 Future Improvements

* Try advanced ML models (Random Forest, XGBoost, LightGBM)
* Add more features (CPU, GPU, Screen size, Company, etc.)
* Deploy on **Heroku / Render / AWS**
* Enhance frontend with modern UI

---

## ✨ Author

👤 **[rushi-0-4](https://github.com/rushi-0-4)**

---


