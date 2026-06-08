🌟 VisionClassifier Pro - User Guide

Welcome to VisionClassifier Pro! This is a complete, modern, and 100% private AI image classifier that runs directly inside your web browser. This guide will help you set up the application, load your custom AI model, and start classifying images in seconds.

🚀 Quick Start

1. Run the Web App

Because browser security prevents loading local files directly from your hard drive, you need to run this app on a local web server.

Here are three simple, safe ways to do it:

VS Code Live Server: If you use VS Code, install the Live Server extension, open index.html, and click the "Go Live" button at the bottom right.

Python Server: If you have Python installed, open your terminal or command prompt in your project folder and run:

python -m http.server 8000


Then, open your web browser and go to http://localhost:8000.

Node.js Server: Install http-server via npm and run it in your project folder:

npx http-server


🧠 How to Load the AI Model

This application supports loading TensorFlow.js models trained with Google's Teachable Machine. We have a pre-trained model ready for you to try!

Direct Model URL: https://teachablemachine.withgoogle.com/models/cs9okuHAJ/

Ways to Load Your Model in the App:

Option A: Cloud URL (Recommended & Easiest)

Open the app in your browser.

Under Model Settings, select the Cloud URL tab.

Paste the direct link: https://teachablemachine.withgoogle.com/models/cs9okuHAJ/ into the input field.

Click the Load button.

Look at the top right header—the status badge will turn green and say "Model Ready"!

Option B: Default Local Folder

If you have downloaded your model files from Teachable Machine:

Create a folder named my_model in the same directory as your index.html file.

Place your downloaded model.json, metadata.json, and weights.bin inside that folder.

The app will automatically attempt to load the model from this folder on startup when using the Default Local tab.

Option C: Upload Files Directly

If you want to test files directly from your computer without setting up folders:

Choose the Upload Files tab in the Model Settings.

Select your model.json, weights.bin, and metadata.json files using the three upload buttons.

Click Initialize Selected Files.

📸 Classifying Images

Once the model status displays "Model Ready", you can choose between two safe, easy input sources:

📁 Method 1: Upload & Drop (Static Images)

Ensure the Upload & Drop tab is selected under Input Source.

Drag and drop any image file (PNG, JPG, WEBP, or GIF) into the dashed box, or click the box to open your file manager and select an image.

The app will immediately display your image preview and show the top-5 predictions on the right, complete with interactive confidence progress bars!

🎥 Method 2: Live Webcam

Select the Live Webcam tab under Input Source.

Click Start Live Stream.

Grant permission to your webcam when prompted by your browser.

Hold objects up to the camera to see real-time classification speed and top predicted classes instantly! Click Stop Stream at any time.

🔒 Privacy & Safety First

On-Device Processing: This application runs entirely inside your browser using your computer's graphics power (WebGL/WASM).

Zero Data Shared: Your images, webcam streams, and data are never uploaded to any external server. Your privacy is fully protected!
