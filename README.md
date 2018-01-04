# Gender recognition by voice
[Statistical learning]:http://edu.epfl.ch/coursebook/fr/statistical-learning-MATH-412$
[Anaconda]:https://anaconda.org/anaconda/python
[Kaggle]:https://www.kaggle.com/primaryobjects/voicegender
Jupyter notebooks for the project "Gender recognition by voice" for the EPFL [Statistical learning] course. The objective is to predict whether a voice recording is 'male' or 'female' based on spectral features extracted from the each recording. The dataset, available on [Kaggle], is a '.csv' file which consists of features extracted 3248 voice recordings.

## Installation
1. Install Python 3.6 and [Anaconda].
1. Create an anaconda environment.
    ```bash
    conda create -n gender_recognition python=3.6
    source activate
    ```
1. Clone or download the repository.
    ```bash
    git clone https://github.com/AdriBesson/Gender_recoginition_speech
    cd Gender_recoginition_speech
    ```
1. Install the python dependencies
    ```bash
    pip install --upgrade pip
    pip install -r requirements.txt
    ```

## Usage
1. Run the different notebooks: the notebooks follow the process described in ``Report_Besson_Lefebvre_Kaklamanos.pdf'':
  .* Gender recognition by voice - data analysis.ipynb: Exploratory data analysis described in Chapter 3
  .* Gender recognition by voice - A first intuitive approach.ipynb: Classification using only the fundamental frequency described in Chapter 4
  .* Gender recognition by voice - Classification with 80-20 split.ipynb: Classification using all the features and a 80/20 split of the dataset. The training set is used for parameter selection and the test set is used to choose the best model. Due to a high variance of the classification error with respect to the split of the dataset, this approach is not able to identify the best model. Described in Chapter 4
  .* Gender recognition by voice - Classification with 50-50 split.ipynb: Classification using all the features and a 50/50 split of the dataset. The training set is used for parameter selection and the test set is used to choose the best model. In order to reduce the variance of the error, we use 5-fold cross validated scores on the test set. This method is able to identify the best model. Described in Chapter 5
