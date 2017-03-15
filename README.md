# Behavioral-Cloning-Hacktorial-Files
All the files needed for the Terrapin Hackers Hacktorial on Behavioral Cloning for Self Driving Cars.

The [model.py](/model.py) is a template for the hacktorial and the final code is available to view in [final_model.py](/final_model.py). [drive.py](/drive.py) contains the code needed to connect your model and the simulator.

Model inspired by [Nvidia's End to End Learning Paper](https://devblogs.nvidia.com/parallelforall/deep-learning-self-driving-cars/). Project idea, [drive.py](/drive.py), and training data from Udacity Self Driving Car Nanodegree program.

## Installation
To run the models and code make sure you [Python](https://www.python.org/downloads/) installed. 

Also make sure you have OpenCV installed either through pip or homebrew. You can check if this works by running and making sure nothing complains:
```
python
import cv2
```
Install all the python dependencies:
```
pip install -r requirements.txt
```
Download Udacity's training data and extract it to the main directory by running in the directory.
```
wget https://www.dropbox.com/s/3cwc2atg1qorzg4/data.zip?dl=0
unzip -a data.zip
```

Download the simulator [here](https://github.com/udacity/self-driving-car-sim).

## View the Instructional Guide Notebook
To view the notebook run
```
jupyter notebook
```
and open [Model_Guide_and_Visualization.ipynb](/Model_Guide_and_Visualization.ipynb)

## Create training data
To create your own training data, open the simulator and select any track and the training option. All the data will be saved to the location you specify.

## Train the Model
To train the model run
```
python model.py
```

## Test Model on Simulator
To run your trained model on the simulator, open up the simulator application and start an autonomous session on either track. Then run
```
python drive.py model.json
```

Nvidia's End to End Model:
![Image of Nvidia Model](/images/nVidia_model.png)
