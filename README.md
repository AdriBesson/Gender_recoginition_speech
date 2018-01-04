# Gender recognition by voice
[Statistical learning]:http://edu.epfl.ch/coursebook/fr/statistical-learning-MATH-412$
[Anaconda]:https://anaconda.org/anaconda/python
[Kaggle]:https://www.kaggle.com/primaryobjects/voicegender
Jupyter notebooks for the project "Gender recognition by voice" for the EPFL [Statistical learning] course. The objective is to predict whether a voice recording is 'male' or 'female' based on spectral features extracted from the each recording. The dataset, available on [Kaggle], is a '.csv' file which consists of features extracted 3248 voice recordings.


## Installation
1. Install Python 3.6 and [Anaconda].
1. Create an anaconda environment.
    ```bash
    conda create -n statistical_learning python=3.6
    source activate
    ```
1. Clone or download the repository.
    ```bash
    git clone https://github.com/AdriBesson/Statistical_learning_course
    cd statistical_learning_course
    ```
1. Install the python dependencies
    ```bash
    pip install --upgrade pip
    pip install -r requirements.txt
    ```

## Usage
1. Go in the desired directory and run jupyter notebook
    ```bash
    cd week1
    jupyter notebook
    ```
1. Run the desired notebook
