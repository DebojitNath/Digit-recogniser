# ✍️ Digit Recognizer (CNN Web App)

A web-based handwritten digit recognition application using a **Convolutional Neural Network (CNN)** trained on the **MNIST dataset**.  
Built with **Django** and **TensorFlow.js** for real-time, browser-based inference.

---

## 🚀 Highlights

- Draw digits (0–9) on an interactive canvas  
- Real-time predictions using a pre-trained CNN  
- Displays confidence scores for all digit classes  
- Client-side inference (no server-side ML execution)

---

## 🛠 Tech Stack

- **Backend:** Django  
- **Frontend:** HTML, CSS, JavaScript  
- **Machine Learning:** TensorFlow.js  
- **Model:** CNN trained on MNIST

---

## 🧠 Model Overview

- Input: 28×28 grayscale images  
- Output: Digits 0–9  
- Architecture: Convolutional Neural Network (CNN)  
- Inference runs directly in the browser

---

## 📁 Project Structure

```
digit-recogniser/
├── api/                    # Django app
│   ├── migrations/         # Database migrations
│   ├── static/api/         # Static files (CSS, JS, model)
│   ├── templates/api/      # HTML templates
│   ├── views.py            # View functions
│   └── urls.py             # URL patterns
├── dlserver/               # Django project settings
├── draw-canvas/            # Additional canvas demo (optional)
├── manage.py               # Django management script
└── README.md
```

## ⚙️ Installation & Setup

```bash
# Clone repository
git clone https://github.com/DebojitNath/Digit-recogniser.git
cd Digit-recogniser

# Install dependencies
pip install django==1.10

# Apply migrations
python manage.py migrate

# Collect static files
python manage.py collectstatic --noinput

# Run development server
python manage.py runserver

# Open your browser and navigate to:
http://127.0.0.1:8000/
```

## 🎯 Use Case

This project demonstrates the integration of **deep learning models with web applications**, showcasing end-to-end ML deployment using browser-based inference.

---

⭐ If you find this project useful, consider starring the repository.
