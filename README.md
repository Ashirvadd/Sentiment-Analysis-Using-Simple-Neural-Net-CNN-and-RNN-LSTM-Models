# Sentiment Classification of IMDb User Reviews with LSTM

This guide provides a comprehensive walkthrough on building a sentiment classification model for IMDb movie reviews using LSTM with Keras and deploying it locally through Flask. We’ll use the IMDb movie reviews dataset available [here](https://www.kaggle.com/datasets/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews).

To identify the best model for this task, we experimented with three architectures: Simple Neural Network, CNN, and LSTM. After evaluating each model, we explain why LSTMs are particularly effective for handling sequential text data.

<img width="791" height="272" alt="Image" src="https://github.com/user-attachments/assets/69aff0c5-ce5e-45d1-891b-f594021461b7" />
<img width="829" height="563" alt="Image" src="https://github.com/user-attachments/assets/0bdcac16-f9a6-4da9-b397-59d1c6cee16a" />
<img width="533" height="240" alt="Image" src="https://github.com/user-attachments/assets/a4caad8c-ebe8-475f-b028-336b8e7c49d6" />
<img width="878" height="287" alt="Image" src="https://github.com/user-attachments/assets/4e858eb4-c535-4d7a-9b5e-6f5d23d02841" />
<img width="1052" height="275" alt="Image" src="https://github.com/user-attachments/assets/31ae53a9-de9d-4be6-b894-41473df13c7c" />
<img width="860" height="351" alt="Image" src="https://github.com/user-attachments/assets/b64c51ed-b6d6-4357-8278-ab3c829a3562" />
<img width="1073" height="271" alt="Image" src="https://github.com/user-attachments/assets/f6d74aed-8b94-4a1f-bce2-b5ce353c7f00" />
<img width="873" height="346" alt="Image" src="https://github.com/user-attachments/assets/932bf8c4-9a9c-4a3f-b585-cb96e79ba944" />
<img width="866" height="291" alt="Image" src="https://github.com/user-attachments/assets/5c0f7272-a464-4878-abd7-889f554fe1ec" />
<img width="1093" height="267" alt="Image" src="https://github.com/user-attachments/assets/4fdccf1e-ac5f-46bc-abc4-6a908dc47324" />
<img width="735" height="670" alt="Image" src="https://github.com/user-attachments/assets/e5a280d3-ca82-4091-a8af-845ea294176e" />
<img width="1375" height="388" alt="Image" src="https://github.com/user-attachments/assets/9c7a2e63-81be-44fb-aeb1-216df06895b3" />
<img width="1313" height="522" alt="Image" src="https://github.com/user-attachments/assets/a5fd3cbc-25f5-4b88-9218-0984f346eceb" />

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
