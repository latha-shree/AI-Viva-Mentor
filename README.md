🎤 AI Viva Mentor

AI Viva Mentor is a Flask-based web application that conducts mock interviews and quizzes. It evaluates candidates based on their spoken answers, measures answer similarity, and uses real-time emotion detection through webcam to assess confidence and engagement.

📖 Features
🔹 AI Interview Evaluation

Conducts a mock viva interview with predefined technical questions.

Candidate speaks answers → converted to text using Google Speech Recognition API.

Compares spoken answers with stored correct answers using text similarity.

Saves results in interview_results.csv with timestamps.

Each new interview automatically deletes the old CSV and creates a new one for fresh results.

🔹 Emotion Detection

Uses OpenCV and a pre-trained Deep Learning model (your_model.keras) to detect emotions in real time.

Recognizes emotions like Happy, Sad, Surprise, Neutral, etc.

Provides feedback based on dominant emotion (e.g., “Student should be more confident”).

🔹 Quiz / Viva Module

Multiple-choice quiz with automated scoring.

Detailed review of correct and incorrect answers after submission.

🔹 Authentication System

Simple signup and login using SQLite (mockemoji.db).

Session-based authentication for secured access.

🛠️ Tech Stack

Backend: Flask (Python)

Database: SQLite

Machine Learning: TensorFlow/Keras (emotion recognition)

Frontend: HTML, CSS, Bootstrap, Jinja2 templates

Other Tools: OpenCV, SpeechRecognition, SoundDevice, Tkinter

▶️ How It Works

Interview Module

Candidate answers viva questions via microphone.

Speech → text conversion using Google Speech Recognition.

Answers compared with expected answers.

Similarity scores calculated and stored in a new CSV each session.

Emotion Detection

Webcam captures candidate’s expressions in real time.

Emotions analyzed frame-by-frame.

Final feedback based on dominant emotion (e.g., Happy → confident).

Quiz Module

Candidate answers multiple-choice questions.

Automated scoring with result breakdown.

📊 Outputs

interview_results.csv

Automatically created fresh for each interview.

Columns:

Timestamp

Question number

Similarity score (%)

Result page displays:

Average similarity score

Dominant emotion

Feedback message

📌 Requirements

Install dependencies:

pip install flask pandas scikit-learn tensorflow keras opencv-python sounddevice soundfile SpeechRecognition pillow

✨ Future Improvements

Add real-time dashboard for candidate performance.

Expand viva question bank dynamically.

Enhance emotion recognition with advanced deep learning models.


![home1](https://github.com/latha-shree/AI-Viva-Mentor/blob/main/home1.png)
![home2](https://github.com/latha-shree/AI-Viva-Mentor/blob/main/home2.png)
![login](https://github.com/latha-shree/AI-Viva-Mentor/blob/main/login.png)
![interview1](https://github.com/latha-shree/AI-Viva-Mentor/blob/main/interview1.png)
![interview2](https://github.com/latha-shree/AI-Viva-Mentor/blob/main/interview2.png)
![int_result](https://github.com/latha-shree/AI-Viva-Mentor/blob/main/int_result.png)
![viva1](https://github.com/latha-shree/AI-Viva-Mentor/blob/main/viva1.png)
![viva2](https://github.com/latha-shree/AI-Viva-Mentor/blob/main/viva2.png)
![viva_res](https://github.com/latha-shree/AI-Viva-Mentor/blob/main/viva_res.png)
![viva_res1]()
![viva_res2]()
