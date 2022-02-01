# About

Exercise Tracker is an ML app that provides users with visual feedback for a set of 6 full-body exercises. The main goal of the app is to encourage users during their workout with the ML model feedback (trying out different exercises and adjusting their form).

How it works: Users view a webcam pop-up that guides them through workouts with real-time exercise form detection. The ML model used for the app shows which exercise the user is currently doing. This is based on how closely their exercise form is to the dataset the model was trained on. A text overlay and moving bar indicates the current exercise the user is doing.

I trained an LSTM neural network in Tensorflow and Keras using my own dataset. The dataset was created by collection full-body keypoint data based on Mediapipe Holistic human topology. This was split into training and testing data for the neural network. The model training code is in the projectsetup notebook.

# How to Run

There are two options for running the exercise tracker:
- open the ExerciseTracker.py file in the command line
- open ExerciseTrackerRunner.ipynb in Jupyter Notebooks and click Run All cells

Once the OpenCV webcam pops up, the program is running, and users can start going through exercises and receive feedback from the ML model.

To exit the exercise tracker, press the key 'q'.

# Tools used:

- Mediapipe Holistic
- Tensorflow
- Keras
- OpenCV
- python
- VSCode