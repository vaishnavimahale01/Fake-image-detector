🕵️‍♂️ Fake Image Detection with ELA and CNN
This project is designed to identify whether images are real or fake using a combination of Error Level Analysis (ELA) and a Convolutional Neural Network (CNN).

🔍 Project Overview
🧪 Error Level Analysis (ELA)
ELA is a technique used to highlight areas within an image that have different levels of compression. When an image is digitally manipulated, the altered regions often compress differently.

The image is resaved at a known compression rate (e.g., JPEG quality 90).
The differences between the original and resaved image are visualized.
These differences can expose tampering and inconsistencies.
🧠 Convolutional Neural Network (CNN)
After ELA processing, the modified images are fed into a CNN. CNNs are particularly effective for image classification tasks due to their ability to learn spatial hierarchies of features.

The CNN learns to distinguish between authentic and tampered images based on the error patterns revealed by ELA.
⚙️ How It Works
🗂️ Dataset Preparation
The dataset contains labeled images, categorized as either real or fake.
Each image is processed using ELA to create a visually enhanced version highlighting manipulated regions.
🧼 Preprocessing
All images are resized (e.g., 128×128) and normalized.
This ensures consistency and improves CNN training performance.
🏋️ Model Training
The CNN is trained on ELA-transformed images and their corresponding labels.
It learns to identify forgery patterns such as localized compression artifacts.
📊 Evaluation
The trained model is evaluated using:
Accuracy metrics
Loss curves
Confusion matrix
🤔 Why Use ELA + CNN?
ELA Exposes Tampering
Subtle digital manipulations become visually and numerically detectable.

CNNs Learn Complex Patterns
The model identifies image manipulations that may not be obvious to the human eye.

💡 Use Cases
🖼️ Detecting forgeries in digital photographs
📰 Authenticating images in journalism, legal, or forensic contexts
🎓 Developing educational tools for teaching digital image integrity
