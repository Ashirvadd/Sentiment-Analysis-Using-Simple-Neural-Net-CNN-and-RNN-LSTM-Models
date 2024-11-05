# Sentiment Classification of IMDb User Reviews with LSTM

This guide provides a comprehensive walkthrough on building a sentiment classification model for IMDb movie reviews using LSTM with Keras and deploying it locally through Flask. We’ll use the IMDb movie reviews dataset available [here](https://www.kaggle.com/datasets/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews).

To identify the best model for this task, we experimented with three architectures: Simple Neural Network, CNN, and LSTM. After evaluating each model, we explain why LSTMs are particularly effective for handling sequential text data.

## How the Model Functions
The model processes each review to predict its sentiment as positive or negative, using an LSTM model optimized for sequential text data. This approach enables the model to capture contextual information across word sequences, leading to more accurate sentiment classification.

## Running the Project on Windows

### Prerequisites
* [Python 3.9](https://www.python.org/downloads/) (add to [PATH](https://medium.com/co-learning-lounge/how-to-download-install-python-on-windows-2021-44a707994013))
* [Git](https://www.markdownguide.org/basic-syntax/)

### Instructions

1. Open Git CMD, navigate to your desired directory, and clone the repository:

       git clone https://github.com/skillcate/sentiment-analysis-with-deep-neural-networks.git 

2. Open Windows PowerShell, navigate to the project folder, and follow these steps to run the Flask application:

   - **Using Conda Environment**:

         conda env create -f conda_env_win.yml   # creates the 'app_env' environment
         conda env list                          # confirms environment creation
         conda activate app_env                  # activates the environment
         python app.py                           # starts the Flask app
         conda deactivate                        # deactivates the environment

   - **Using PIP and Virtualenv**:

         pip install virtualenv                  # installs virtual environment
         virtualenv ENV                          # creates environment named ENV
         .\ENV\Scripts\activate                  # activates ENV
         pip install -r pip_requirements.txt     # installs dependencies
         python app.py                           # starts the Flask app
         deactivate                              # deactivates ENV

## Running the Project on Mac

### Prerequisites
* [Python 3.9](https://www.python.org/downloads/)

### Instructions

1. Open Terminal, navigate to your desired directory, and clone the repository:

       git clone https://github.com/skillcate/sentiment-analysis-with-deep-neural-networks.git 

2. Move to the project directory and follow these steps to run the Flask application:

   - **Using Conda Environment**:

         conda env create -f conda_env_mac.yml   # creates 'app_env'
         conda env list                          # confirms environment creation
         conda activate app_env                  # activates the environment
         python app.py                           # starts the Flask app
         conda deactivate                        # deactivates the environment

   - **Using PIP and Virtualenv**:

         pip install virtualenv                  # installs virtual environment
         virtualenv ENV                          # creates environment named ENV
         source ENV/bin/activate                 # activates ENV
         pip install -r pip_requirements.txt     # installs dependencies
         python app.py                           # starts the Flask app
         deactivate                              # deactivates ENV

## Reporting Issues or Feature Requests
If you encounter any issues (e.g., incorrect results or crashes), please submit a report [here](https://github.com/skillcate/sentiment-analysis-with-deep-neural-networks/issues). Include any relevant details to help address the issue.