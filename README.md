# TruthLens
🧠 Deepfake Detector with Interactive Feedback and Fine-Tuning
An AI-powered web app that detects whether an image is FAKE or REAL, and learns from user feedback in real-time.

This project uses a fine-tuned transformer model to classify deepfake images, and includes a feedback mechanism where users can correct misclassifications — allowing the model to fine-tune itself on-the-fly without manual retraining.

🔍 Features
🖼️ Upload any image (JPG, PNG, etc.)

✅ Instant prediction: REAL or FAKE

📝 If prediction is wrong, user can correct the label

🔁 Model automatically fine-tunes on corrected input

💾 Saves the updated model locally

⚡ Simple and clean Gradio interface

🚀 Technologies Used
Gradio – Fast web interface for ML models

Transformers – Model loading and image processing (SigLIP)

Torch – Training backend

PIL – Image handling

🛠 Setup Instructions
Clone this repo:

bash
Copy
Edit
git clone https://github.com/your-username/deepfake-feedback-app.git
cd deepfake-feedback-app
Install dependencies:

bash
Copy
Edit
pip install -r requirements.txt
Run the app:

bash
Copy
Edit
python app.py
Or try it in Google Colab (for GPU support).

📦 Model Used
prithivMLmods/deepfake-detector-model-v1

🧠 Feedback Loop
The model uses the user-corrected label to fine-tune itself for 1 epoch using AdamW. This makes the app suitable for continual learning and human-in-the-loop AI scenarios.

📸 Screenshot
Add a screenshot of the Gradio interface here.

✨ Future Work
Deploy on Hugging Face Spaces

Add session-based memory of predictions

Include confidence scores in output

🔗 License
MIT License
