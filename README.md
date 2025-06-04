1. What This Project Does and Why I Chose This Project:

This project develops an automated deep learning system to detect breast cancer from medical images, enabling early and accurate diagnosis. It helps reduce human error and speeds up screening, supporting radiologists.
I chose this project because breast cancer is a major health issue, and using AI for early detection aligns with my passion for healthcare technology and creating real-world impact.

2. How My Project Solves This Problem

The project uses CNNs to classify breast ultrasound images as benign or malignant by automatically extracting features. Grad-CAM is applied to highlight important image regions, improving model interpretability and
helping doctors understand AI decisions.

3. Technologies and Frameworks Used in This Project
   
Python, TensorFlow / Keras, PyTorch, OpenCV / PIL, NumPy / Pandas, Matplotlib / Seaborn, Kaggle Notebook, Scikit-learn 

4. Dataset Chosen and Basis of Selection

The project uses a publicly available Breast Ultrasound Images Dataset containing labeled benign and malignant cases. The dataset features high-quality, diverse grayscale images with balanced classes, making it 
suitable for effective deep learning training and reflecting real clinical variations.

5. Working of the Project and Description of All Models

The core workflow:
a) Data Preprocessing- Images are resized, normalized, and augmented to improve model robustness.
b) Model Training- Several CNN architectures were trained and compared:
  Custom CNN- A simple convolutional neural network designed from scratch.
  ResNet (Residual Network)- A deep CNN with skip connections to improve gradient flow.
  EfficientNet- A CNN architecture optimized for performance with fewer parameters.
Each model outputs a binary classification: benign or malignant.
Model Evaluation- Models are assessed using accuracy, precision, recall, F1-score, and ROC-AUC.
Interpretability with Grad-CAM- Grad-CAM generates heatmaps over input images to highlight important regions influencing the classification.

8. Why I Chose Grad-CAM
Grad-CAM was chosen to address the black-box nature of deep learning models. While CNNs can achieve high accuracy, their lack of transparency limits clinical trust. Grad-CAM provides a visual explanation by 
producing heatmaps that localize regions in the image responsible for the model’s decision. This helps doctors validate whether the model focuses on medically relevant features like tumors or suspicious tissue, 
increasing trust and facilitating model acceptance in medical practice.

9. Effect of Implementing Grad-CAM on Results
Implementing Grad-CAM enhanced the interpretability of the results without compromising classification accuracy. It enabled visualization of decision-making areas, providing insight into model behavior and 
identifying potential failure cases. It also helped in debugging and refining the model by revealing if irrelevant image regions influenced predictions. Overall, Grad-CAM increased the project’s clinical usability
by bridging AI predictions with human expert validation.

10.  Final Output and Conclusion
The final output is a notebook that takes breast ultrasound images as input and predicts whether the image shows benign or malignant tissue. It also outputs Grad-CAM heatmaps to highlight suspicious regions for the
user.


