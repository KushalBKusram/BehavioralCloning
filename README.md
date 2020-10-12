# Behavioral Cloning

## Description
A neural network designed to learn and clone car driving behavior in autonomous mode in Udacity Self Driving Car Simulator. The network is designed as a supervised regression problem between the car steering angles and road images from the car. The network is _ layers deep. The network predicts an angle for the car to manuever based on the input from camera in front of the car.

During training, images from three different camera angles (from the center, the left and the right of the car are used.

## Documentation
### Project Directory
**src:** The main project directory. The network and its training related functions are contained in [model.py](https://github.com/KushalBKusram/BehavioralCloning/blob/main/src/model.py). The runtime inference and running a Flask app in the background are contained in [drive.py](https://github.com/KushalBKusram/BehavioralCloning/blob/main/src/drive.py). <br/>
**data:** You have to create this directory within this parent directory to store images for training from Udacity Self Driving Car Simulator. <br/>
**model:** Consists of a model that was training on the data that I collected and should drive the car around the simple and easy track without crashing. It also consists a visual representation of the network exported after training by model.py.

## Requirements
Python 3 and above, OpenCV 3 or above, NumPy, MoviePy, TensorFlow, Keras, Flask. There might be certain dependencies that may not be present in your environment. Hence, it is recommended that you setup a new virtual environment with help of [requirements.txt](https://github.com/KushalBKusram/BehavioralCloning/blob/main/requirements.txt)

## Usage
### Training
For training, the program assumes that training images and corresponding file with steering angles are present in "data"

```python
python model.py
```

### Runtime
For runtime inference, start drive.py first and then enter autonomous mode in the simulator.

```python
python drive.py model.h5
```

For a detailed explanation, please refer to my [article]() on Medium to get started with this repository.

## License
Licensed under the [MIT License](https://github.com/KushalBKusram/BehavioralCloning/blob/main/LICENSE).
