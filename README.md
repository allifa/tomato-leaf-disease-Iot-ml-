# tomato-leaf-disease-Iot-ml-
This project introduces an innovative approach combining IoT and Machine Learning to address this issue. We use an ESP32-CAM module to capture high-resolution images of leaves, which are uploaded to Google Drive. A pre-trained Machine Learning (ML) model processes these images to identify whether the leaf is healthy or affected by any of the five diseases it has been trained to recognize. The ML model, trained on a dataset of over 1000 labeled images, ensures high accuracy in predictions. 
## Implementation
Image Capture: The ESP32-CAM is programmed using Arduino IDE to capture leaf images. Once powered on, it uses its built-in Wi-Fi module to connect to a network and upload images to Google Drive via the Google Drive API.
Model Training: The ML model was trained using TensorFlow on a dataset of over 1000 images. The dataset included five categories: healthy leaves and four diseased types (name the diseases if possible). The training involved preprocessing, data augmentation, and optimizing the CNN architecture for higher accuracy.
Integration: The system integrates the hardware and software by automating image upload and retrieval, enabling real-time analysis.
## Working
Step 1: The ESP32-CAM captures an image when powered on or triggered. 
Step 2: The image is uploaded to a dedicated folder in Google Drive.
Step 3: The ML model, running on Google Colab, retrieves the image, preprocesses it, and classifies it.
Step 4: The result (e.g., "Healthy" or "Infected with Disease X") is sent back to the farmer via a web interface or SMS.

