# StimulEye
Classifying raw streams of eye tracking data from an eye tracker and analysing it to classify the inputs into eye gaze events, namely Saccades, Fixations and Blinks.

Abstract: Extraction of eye gaze events is highly dependent on automated powerful software that charge exorbitant prices. This is an open source tool-StimulEye that helps to detect and classify eye gaze events and analyse various metrics related to these events. StimulEye uses deep learning techniques to automate eye gaze event detection that does not require decision making or parametric definitions by humans. The tool aims to provide an end to end solution which takes  raw streams of eye tracking data from an eye tracker and analyses it to classify the inputs into the events, namely Saccades, Fixations and Blinks.

To run this tool, you can either upload the file online to a Google Colab file, upload the data set and run it in a sequence.

To run this tool locally on your desktop, Follow the following steps:
Setup a Python virtual environment. Setup a separate, sequestered python environment for this project.
Install virtualenv and virtualenvwrapper. Both are pip installable.
Create a Python 3 virtual environment exclusively for this Keras+TensorFlow based project
$ mkvirtualenv <Name_your_environment> -p python3
Navigate to that virtual environment
$ workon <virtual_env_name>
Install Tensorflow
$ pip install --upgrade tensorflow
Please note that this step will only work if you have a tensorflow compatible graphics card
Pip install all the other dependencies mentioned below:
Keras, csv, math, pandas, numpy, matplotlib, sklearn

Import the .ipynb file into your Jupiter Notebook and run the program. Two files are generated in the directory where your file is located.

1stResultantcsv.csv and 2ndResultantcsv.csv- The initial results of this analysis are stored in the first csv file where each gaze point is classified as Blink, Saccade and Fixation. The second csv file denotes all the fixation points of the dataset. The second csv file contains various information about the fixation points such as fixation centroids (X and Y coordinates), fixation duration and fixation radius.

