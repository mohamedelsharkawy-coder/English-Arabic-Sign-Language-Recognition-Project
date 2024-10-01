# Sign Language Recognition Mobile App

## Overview
The Sign Language Recognition mobile app is designed to facilitate communication between deaf-mute individuals and those who can hear. The app provides features for recognizing both Arabic and English sign languages, making it easier for users to communicate through video and voice.

## Features
- **Dual Language Support:** Provides recognition for approximately 90 words in both Arabic and English sign languages.
- **Video-to-Text Conversion:** Allows deaf-mute users to record a video of their sign language, which is then converted to its equivalent text.
- **Voice-to-Video Conversion:** Enables hearing users to record their voice, which is converted to text using an API, and subsequently turned into a video of corresponding sign language.
- **User-Friendly Interface:** Offers an intuitive mobile interface that enhances the user experience.

## Collaboration
This project was developed in collaboration with Abdelrahman, where I was responsible for the AI development, and he focused on mobile app development.

## AI Development
The AI development was divided into two sections: **English Sign Language** and **Arabic Sign Language**. Each section follows a similar workflow:

### English Section
- The English sign language components are documented in the file `english_project.ipynb`.

### Arabic Section
- The Arabic sign language components are documented in the file `arabic_project.ipynb`.

### Workflow Steps

1. **Dataset Collection:**
   - Collected approximately 360,000 frames (2000 frames for each of the 90 classes) using OpenCV.

2. **Data Cleaning:**
   - Cleaned frames using MediaPipe to remove any blurred images and ensure hands were detected.

3. **Feature Extraction:**
   - Extracted hand landmarks in each frame using MediaPipe and saved them in a pickle file (`english_data.pickle` for the English section and `arabic_data.pickle` for the Arabic section).

4. **Data Splitting:**
   - Split the dataset into training (80%) and testing (20%) sets using Scikit-learn.

5. **Model Building and Training:**
   - Trained a Random Forest Classifier on the training data and saved the model in a pickle file (`english_model.pickle` for the English section and `arabic_model.pickle` for the Arabic section).

6. **Model Evaluation:**
   - Evaluated the model on the test data, achieving an accuracy of 99.8%.

7. **Video Testing:**
   - Developed a prediction mechanism to handle video input by classifying frames and determining which frames to display based on a defined threshold.

8. **Model Deployment:**
   - Deployed the model as a REST API using Flask, making it accessible via Ngrok for the mobile app.

### Text-to-Video Process
1. **Sign Language Video Storage:**
   - Stored videos for each letter and word used in the project.

2. **Voice-to-Text Conversion:**
   - After converting voice input to text, the text is split into individual words.

3. **Video Concatenation:**
   - For each word, corresponding videos are concatenated. If a video for a specific word isn't found, the word is split into its letters, and videos for each letter are used instead.

4. **API Deployment:**
   - This process is deployed as a REST API using Flask, also accessible via Ngrok.

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/mohamedelsharkawy-coder/English-and-Arabic-Sign-Language-Recognition-Project
   cd English-and-Arabic-Sign-Language-Recognition-Project

2. Install Packages:
   ```bash
   pip install -r requirements.txt

