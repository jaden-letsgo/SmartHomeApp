
# Smart Home Application - Gesture Recorder

## Author
Jiahui Li\
(Email: Jiahui15@asu.edu)

## Purpose
The purpose of this project is to develop a mobile application that can record labeled gesture videos for training machine learning models. This project is being completed as a requirement for the ASU MCS 535 course curriculum.

## Background
The Gesture Recorder application is designed to record labeled gesture videos using an Android mobile device or tablet. The recorded videos will be used as training data for a machine learning model that will be developed in part two of this project using TensorFlow. The application has a simple interface that enables users to start and stop video recording, label the gesture they are performing, and save the video to a designated folder using Flask to mimic a remote server. 

## Features
The Gesture Recorder application includes the following features:

* Simple interface for easy recording and labeling of gesture videos
* View an example guesture with the ability to replay the example video
* A record button and a done button for video recording
* Capability to label the gesture being performed in the video
* Save the recorded videos to a designated folder using Flask to mimic a remote server

## Requirement
* [Android Studio](https://developer.android.com/)
* [Python](https://www.python.org/)
* [Flask](https://flask.palletsprojects.com/en/2.2.x/)

## Setup
* Android Studio:
  * Prefer Device Emulator Setup:
    * Pixel 5, API 31, Back Camera: Webcam, Ram: 4 GB+, Internal Storage: 1 GB+

* Flask:
  * Change line 9 and 25 of the [flask_server](https://github.com/jaden-letsgo/SmartHomeApp/blob/main/flask_server.py) file to your designated folder path
  * Please follow [Flask offical guide](https://flask.palletsprojects.com/en/2.2.x/installation/#virtual-environments
) to setup a virtual environments to run flask_server

* Application Code:
   * After runing flask_server, an output should be shown as follow:
    * Running on all addresses (0.0.0.0)
    * Running on http://127.0.0.1:5000
    * Running on http://19*.***.*.**:5000 
    *  Change line 244 of [Pratice.kt](https://github.com/jaden-letsgo/SmartHomeApp/blob/main/app/src/main/java/com/example/smarthomeapp/Pratice.kt) to the ip shown in your device

## Run
1. Ensure flask_server is running
2. Clone the repository: git clone https://github.com/jaden-letsgo/SmartHomeApp.git to Andriod Studio
3. Build and run in Andriod Studio with the appropriate device emulator

## Usage
To use the Smart Home Application, follow these steps:

### Landing Page
* From the drop down menu, select the desire guesture to record

### Example Video Viewing Page
* The Video should play automically
* Click replay button to replay video

### Recording Page
* Pressing Record button will start recoring
   * Recording is timed and will be ended in 5 seconds
* Press Record to repeat recording process
* Press Done to go back to the first page to select next guesture

## Contributing

Android app is a free and open source project, any contributions are welcome!

### Making change

If any changes are make without any notification to code owner, please create new branch and make a pull request with the new branch.

For contributions via GitHub, see the [GitHub Contribution Guide](CONTRIBUTING.md).

### Accepted Types of Contributions
* Bug fixes
* Each bug fix is expected to come with tests
* Fixing spelling errors
* Adding new tests to the area that is not currently covered by tests
* New features
* Add or improve question and answer
* Code logic to improve time complexity and/or dynamic capabilities

## Right to the project

Initial constributors: Jiahui Li

### Using the project

This Project is strictly to be use for non-commercial purpose only. No Exception!

### Right to resource used in the project

Some of the used libraries are released under different licenses.
