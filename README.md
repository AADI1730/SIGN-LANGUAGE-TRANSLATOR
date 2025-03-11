Sign Language to Text & Speech Recognition

This project detects hand signs in real-time, converts them into text, and optionally speaks the recognized sign using Machine Learning and Computer Vision.

🚀 Features

✅ Real-time hand gesture recognition using OpenCV & MediaPipe✅ ML Model Training for sign classification✅ Converts recognized signs to text✅ Text-to-Speech (TTS) conversion using pyttsx3

📂 Project Structure

📁 Sign-Language-to-Text-and-Speech
│── 📂 data/               # Stores images for training
│── 📂 myenv/              # Virtual environment (optional)
│── 📝 requirements.txt     # List of dependencies
│── 📝 README.md            # Project documentation
│── 📝 .gitignore           # Git ignored files
│── 📜 createDataset.py     # Extracts features & creates `data.pickle`
│── 📜 trainClassifier.py   # Trains ML model & creates `model.p`
│── 📜 main.py              # Runs real-time sign recognition
│── 📜 model.p              # Saved trained model
│── 📜 data.pickle          # Processed dataset

🛠 Installation & Setup

Step 1: Clone the Repository

git clone [https://github.com/YourUsername/Sign-Language-to-Text-and-Speech.git
cd Sign-Language-to-Text-and-Speech](https://github.com/AADI1730/SIGN-LANGUAGE-TRANSLATOR)

Step 2: Set Up a Virtual Environment

python -m venv myenv
source myenv/bin/activate  # On Mac/Linux
myenv\Scripts\activate      # On Windows

Step 3: Install Dependencies

pip install -r requirements.txt

🔄 Dataset Preparation

Collect Sign Images:Run the following script to capture images:

python collectImgs.py

Create the Dataset (data.pickle):

python createDataset.py

Train the Model (model.p):

python trainClassifier.py

🏃 Running the Project

Once the model is trained, run the real-time sign recognition:

python main.py

Camera will open 📷

Show a hand sign, and it will display & speak the recognized sign 🗣️

🧠 Technologies Used

Python 🐍

OpenCV (Computer Vision)

MediaPipe (Hand Tracking)

Scikit-Learn (ML Model)

Pyttsx3 (Text-to-Speech)

📌 Troubleshooting

FileNotFoundError: No such file data.pickle

Fix: Run:

python createDataset.py

Model always predicts "J"

Add more diverse images

Retrain with trainClassifier.py

📢 Contributors

Aditya kumar (https://github.com/AADI1730)

📜 License

This project is licensed under the MIT License.

