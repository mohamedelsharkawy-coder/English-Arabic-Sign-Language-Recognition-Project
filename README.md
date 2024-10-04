# 🤟 English_Arabic Sign Language Recognition Project

Hello👋, I'm Mohamed Elsharkawy, a Data Science and AI enthusiast 🤖❤️. I recently completed an English and Arabic Sign Language Recognition project 🧑‍💻✨ as a scaling up for my previous [Real-Time-American-Sign-Language-Recognition](https://github.com/mohamedelsharkawy-coder/Real-Time-American-Sign-Language-Recognition), furthering my skills in computer vision 🌟. This project was a big step in my learning journey into AI 📚, and I'm always seeking improvement through self-learning and creating projects 🔧⚒️.

🙏 Thank you for visiting my repository! I hope you find this project helpful and informative 💡📘.
## 📖 Overview
It is a Sign Language Recognition mobile app that designed to facilitate communication between deaf-mute individuals and those who can hear. The app provides features for recognizing both Arabic and English sign languages, making it easier for users to communicate through video and voice.

## 🚀 Features
- **Dual Language Support:** Provides recognition for approximately 90 words in both Arabic and English sign languages. 🌐
- **Video-to-Text Conversion:** Allows deaf-mute users to record a video of their sign language, which is then converted to its equivalent text. 🎥➡️📜
- **Voice-to-Video Conversion:** Enables hearing users to record their voice, which is converted to text using an API, and subsequently turned into a video of corresponding sign language. 🎤➡️📜➡️🎞️
- **User-Friendly Interface:** Offers an intuitive mobile interface that enhances the user experience. 📱✨

## 🛠️ Technologies Used
This project utilizes a variety of powerful libraries and frameworks to implement the sign language recognition functionality:

- **Scikit-learn:** A robust machine learning library in Python that provides simple and efficient tools for data mining and data analysis. It was used for model training and evaluation. 📊
  
- **NumPy:** A fundamental package for scientific computing in Python, enabling efficient numerical operations on large, multi-dimensional arrays and matrices. It was essential for data manipulation. 🔢

- **OpenCV:** An open-source computer vision and machine learning software library that provides tools for image and video processing. It was used for dataset collection and video analysis. 🎥

- **MediaPipe:** A cross-platform framework for building multimodal applied machine learning pipelines. It was utilized for hand detection and landmark extraction in sign language recognition. ✋

- **Pickle:** A Python module used for serializing and deserializing Python objects. It was used to save and load the trained models and extracted data efficiently. 📦

- **Matplotlib:** A plotting library for the Python programming language and its numerical mathematics extension NumPy. It was used for visualizing data and results during development. 📈

- **Flask:** A lightweight WSGI web application framework in Python that is easy to use for building web applications. It was employed to create the REST API for model deployment. 🌐

- **Google Colab:** A cloud-based Jupyter notebook environment that allows for the execution of Python code in the browser. It was used for developing and testing the AI models collaboratively. ☁️

- **Jupyter Lab:** An interactive development environment for notebooks, code, and data. It provided a versatile interface for data exploration and model development. 📓

## 🎥 Demo
Check out the demo GIF to see the Sign Language Recognition mobile app in action! This GIF showcases the app's features, including how it converts sign language to text and vice versa.

![Demo Video](media/video.gif)

For a better viewing experience, you can click this link: [Watch the Demo MP4](https://drive.google.com/file/d/1dpS6O1P8uFm-WSuM2QNBC06YX3xBNLui/view?usp=sharing)

## 🤝 Collaboration
This project was developed in collaboration with my friend [Abdelrahman](https://github.com/Abdokarawia), where I was responsible for the AI development, and he focused on mobile app development.

## 🧠 AI Development
The AI development was divided into two sections: **English Sign Language** and **Arabic Sign Language**. Each section follows a similar workflow:

### 🔤 English Section  
The English sign language components are documented in the file `english_project.ipynb`.

### 🕌 Arabic Section
The Arabic sign language components are documented in the file `arabic_project.ipynb`.

### 🔄 Video-to-Text Process

1. **Dataset Collection:**
   - Collected approximately 360,000 frames using OpenCV, with 2,000 frames per class for 90 classes in both English and Arabic sign languages (2 languages × 90 classes × 2,000 frames = 360,000). 📊

2. **Data Cleaning:**
   - Cleaned frames using MediaPipe to ensure hands were detected. 🧹

3. **Feature Extraction:**
   - Extracted hand landmarks in each frame using MediaPipe and saved them in a pickle file (`english_data.pickle` for the English section and `arabic_data.pickle` for the Arabic section). 📦
[Access the pickled data from this link](https://drive.google.com/drive/folders/1KavCk5ktwkwO3dUtO03pRv-4dJTWb6ly?usp=sharing)

4. **Data Splitting:**
   - Split the dataset into training (80%) and testing (20%) sets using Scikit-learn. 🔍

5. **Model Building and Training:**
   - Trained a Random Forest Classifier on the training data and saved the model in a pickle file (`english_model.pickle` for the English section and `arabic_model.pickle` for the Arabic section). 📈

6. **Model Evaluation:**
   - Evaluated the model on the test data, achieving an accuracy of 99.8%! 🎉

7. **Video Testing:**
   - Developed a prediction mechanism to handle video input by classifying frames and determining which frames to display based on a defined threshold. 🎬

8. **Model Deployment:**
   - Deployed the model as a REST API using Flask, making it accessible via Ngrok for the mobile app. 🌐

### 🔄 Text-to-Video Process
1. **Sign Language Video Storage:**
   - Stored videos for each letter and word used in the project. 💾

2. **Voice-to-Text Conversion:**
   - After converting voice input to text, the text is split into individual words. 🔤

3. **Video Concatenation:**
   - For each word, corresponding videos are concatenated. If a video for a specific word isn't found, the word is split into its letters, and videos for each letter are used instead. 🔗

4. **API Deployment:**
   - This process is deployed as a REST API using Flask, also accessible via Ngrok. 🚀

## 🛠️ Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/mohamedelsharkawy-coder/English-Arabic-Sign-Language-Recognition-Project
   cd English-Arabic-Sign-Language-Recognition-Project
   
2. Download packages:
   ```bash
   pip install -r requirements.txt

## 📞 Contact Information

Feel free to reach out if you have any questions, suggestions, or would like to collaborate!

- **Email:** [mohamed.k.elsharkawy@gmail.com](mailto:mohamed.k.elsharkawy@gmail.com)
- **Phone:** +20 100 462 2244
- **LinkedIn:** [Mohamed Elsharkawy's LinkedIn Profile](https://www.linkedin.com/in/mohamed-elsharkawy-6184b41a7/)
- **Kaggle:** [Mohamed Elsharkawy's Kaggle Profile](https://www.kaggle.com/mohamedelsharkawy89)


