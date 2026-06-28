#  Face Recognition System using OpenCV & Python

##  Project Overview

This project is a **Real-Time Face Recognition System** built using **Python** and **OpenCV**. It captures facial data through a webcam, trains a model using the **LBPH (Local Binary Patterns Histogram)** algorithm, and recognizes faces in real-time.

The system supports **incremental learning**, meaning you can add new faces without retraining the model from scratch.

---

##  Features

*  Real-time face detection using Haar Cascades
*  Face recognition using LBPH algorithm
*  Add new users dynamically
*  Update existing trained model
*  Store user data using JSON
*  Confidence score display

---

##  Tech Stack

* **Python**
* **OpenCV**
* **NumPy**
* **JSON**
* **Haar Cascade Classifier**
* **LBPH Face Recognizer**

---

##  Project Structure

```
├── train.py        # Script to capture faces & train/update model
├── main.py         # Script for real-time face recognition
├── names.json      # Stores ID-name mappings
├── my_model.yml    # Trained face recognition model
```

---

##  How It Works

###  Training Phase (`train.py`)

* Takes user input (person's name)
* Captures 30 face samples via webcam
* Converts images to grayscale
* Detects faces using Haar Cascade
* Trains or updates the LBPH model
* Saves model (`my_model.yml`) and names (`names.json`)

###  Recognition Phase (`main.py`)

* Loads trained model and stored names
* Captures live video from webcam
* Detects faces in real-time
* Predicts ID and confidence
* Displays recognized name with confidence score

---

##  How to Run

###  Prerequisites

Make sure you have Python installed along with required libraries:

```bash
pip install opencv-python opencv-contrib-python numpy
```

---

###  Step 1: Train the Model

```bash
python train.py
```

* Enter the person's name
* Look at the camera for face capture

---

###  Step 2: Run Face Recognition

```bash
python main.py
```

* Press **ESC** to exit

---

##  Output

* Recognized faces will be labeled with:

  * **Name**
  * **Confidence Percentage**
* Unknown faces will be labeled as **"Unknown"**

---

##  Key Learnings

* Real-time image processing
* Face detection & recognition techniques
* Model training and updating
* Working with OpenCV modules
* Handling structured data using JSON

---

##  Future Improvements

* Add GUI interface
* Improve accuracy using Deep Learning models (e.g., CNN)
* Store data in database instead of JSON
* Add attendance system integration
* Deploy as a web application

---

##  Contributing

Contributions are welcome! Feel free to fork this repo and submit a pull request.

---

##  Contact

If you have any suggestions or feedback, feel free to connect!

---

