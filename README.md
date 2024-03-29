# Promoter Gene Sequences Classifier

## Overview
This Django web application classifies DNA sequences as promoters using a neural network model trained on the UCI Machine Learning Repository's promoter gene sequences dataset. This project demonstrates an end-to-end machine learning workflow, from data preprocessing and model training to deploying the model in a web application for real-time predictions.

## Getting Started

### Prerequisites
Before you begin, ensure you have the following installed:
- Python 3.8 or higher
- pip and virtualenv

### Installation

### Installation

1. Clone the repository:
   ```sh
   https://github.com/isurulkh/Promoter-Gene-Sequences-Classifier.git
2.**Create a virtual environment:**

  ```bash
  python -m venv venv
  
  ```
3.**Create a virtual environment:**

  * **Windows**
    ```bash
    .\venv\Scripts\activate
    ```
  
 *  **Mac**
    ```bash
    source venv/bin/activate
    ```

4.**Install dependencies:**

  ```bash
  pip install -r requirements.txt
  
  ```

Setting Up the Django Project
Follow these steps to set up and configure your Django project:

Create a Django Project:

```bash
django-admin startproject mysite

```

Navigate to Your Project Directory:
```bash
cd mysite
```

Create a Django Application:
```bash
python manage.py startapp polls
```

Configure Your Application:
Update the settings.py file within the mysite directory to include your new app and any additional configuration needed.

Initialize the Database:
Run migrations to set up your database schema:

```bash
python manage.py migrate
```

Run the Development Server:
Start the Django development server to see if everything is set up correctly:

```bash
python manage.py runserver
Visit http://127.0.0.1:8000/home in your browser to view the site.
```

## Training the Model
The model training script (model_training.ipynb) is included in the repository. To train the model:

Download the promoter gene sequences dataset from the UCI Machine Learning Repository.
Follow the instructions in the Jupyter Notebook to preprocess the data, train the neural network model, and evaluate its performance.
After training, save the model and the one-hot encoder to the specified directory. These will be loaded by the Django application to make predictions.

## Usage
With the server running, navigate to the application's URL to input DNA sequences and receive predictions. The web interface provides a simple form where users can submit sequences to be classified as promoters or non-promoters.

## Contributing
Contributions to this project are welcome! Please fork the repository and submit a pull request with your improvements.

## License
This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments
UCI Machine Learning Repository for providing the dataset.
Django Documentation for guidance on setting up the project.
Scikit-learn Documentation for model training and evaluation techniques.

