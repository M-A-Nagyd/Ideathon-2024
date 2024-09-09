# Investment Guidance

## Overview

The **Investment Guidance** project is a web application designed to provide investment predictions based on historical stock and cryptocurrency data. Users can input their personal details and investment parameters to receive predictions on future investment values. The application uses machine learning models to analyze historical data and generate predictions.

## Features

- **Interactive Web Form**: Input personal details, investment amount, and investment period to get predictions.
- **Background Video**: Engaging video background for a visually appealing interface.
- **Machine Learning Predictions**: Utilizes LSTM neural networks to predict future values.
- **Data Integration**: Fetches data from Yahoo Finance for stock and cryptocurrency analysis.

## Technologies

- **Frontend**: HTML, CSS
- **Backend**: Flask (Python)
- **Machine Learning**: TensorFlow (Keras), scikit-learn
- **Data Source**: Yahoo Finance API
- **No Database**: The application does not use a database.

## Setup and Installation

### Prerequisites

- Python 3.x
- Flask
- TensorFlow
- scikit-learn
- yfinance
- pandas
- numpy

### Installation Steps

1. **Clone the repository**:

    ```bash
    git clone https://github.com/yourusername/investment-guidance.git
    cd investment-guidance
    ```
    
2. **Install the required packages**:

    ```bash
    pip install -r requirements.txt
    ```

3. **Download or train machine learning models**:

    Ensure that model files named `model_<symbol>.h5` are present in the project directory. If they are not, the application will train new models automatically when it runs.

4. **Run the Flask application**:

    ```bash
    python app.py
    ```

    The application will be available at `http://127.0.0.1:5000/`.

## Usage

1. Open a web browser and navigate to `http://127.0.0.1:5000/`.
2. Fill out the form with your name, age, investment amount, and investment period.
3. Click the "Predict" button to submit the form and receive predictions.
4. View the predicted returns on the results page.

## File Structure

- `app.py`: Main Flask application file that contains backend logic.
- `templates/`: Directory for HTML templates.
  - `index.html`: Contains the form for user input.
  - `result.html`: Displays the prediction results.
- `static/`: Directory for static files (currently not used).
- `requirements.txt`: Lists the Python dependencies required for the project.
- `model_<symbol>.h5`: Machine learning model files (if they exist).

## Contributing

Contributions to the project are welcome. To contribute, please fork the repository, make changes, and submit a pull request. For reporting issues or suggesting improvements, please use the Issues tab on GitHub.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more information.

## Acknowledgments

- [Yahoo Finance API](https://www.yahoofinanceapi.com/) for financial data.
- [TensorFlow](https://www.tensorflow.org/) and [Keras](https://keras.io/) for machine learning.
- [Flask](https://flask.palletsprojects.com/) for web application framework.

---
