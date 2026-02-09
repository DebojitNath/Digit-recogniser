# Digit Recognizer

A web-based application for recognizing handwritten digits using a Convolutional Neural Network (CNN) trained on the MNIST dataset. Built with Django backend and TensorFlow.js for client-side inference.

## Features

- Interactive canvas for drawing digits
- Real-time digit recognition using pre-trained CNN model
- Display of prediction probabilities for all digits (0-9)
- Clean, responsive web interface
- No server-side processing required for predictions

## Technologies Used

- **Backend**: Django 1.10
- **Frontend**: HTML5, CSS3, JavaScript
- **Machine Learning**: TensorFlow.js
- **Model**: Pre-trained CNN on MNIST dataset

## Installation

1. **Clone the repository:**
   ```bash
   git clone [<repository-url>](https://github.com/DebojitNath/Digit-recogniser/)
   cd digit-recogniser
   ```

2. **Install Python dependencies:**
   ```bash
   pip install django==1.10
   ```

3. **Run migrations:**
   ```bash
   python manage.py migrate
   ```

4. **Collect static files:**
   ```bash
   python manage.py collectstatic --noinput
   ```

5. **Run the development server:**
   ```bash
   python manage.py runserver
   ```

6. **Open your browser and navigate to:**
   ```
   http://127.0.0.1:8000/
   ```

## Usage

1. Draw a digit (0-9) on the canvas using your mouse or touch input
2. Click the "Predict" button to get the recognition result
3. View the predicted digit and confidence scores for all classes
4. Use the "Clear" button to reset the canvas

## Project Structure

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

## Model Details

- **Architecture**: Convolutional Neural Network
- **Dataset**: MNIST (handwritten digits)
- **Input**: 28x28 grayscale images
- **Output**: 10 classes (digits 0-9)
- **Framework**: TensorFlow.js for browser-based inference

## Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- MNIST dataset by Yann LeCun and Corinna Cortes
- TensorFlow.js team for the amazing library
- Django community for the robust web framework

