# LW4_Improving-CNN-Performance

<h3>Activity 1: Evaluation Metrics + Visualization</h3>
<p>https://colab.research.google.com/drive/1o0AilPAWzaSBxLBi-m0NcEtiJUTZFgtM#scrollTo=y9a2-HYbSA-j&line=1&uniqifier=1</p>
<h3>Activity 2: Model Interpretability using
Gradient-weighted Class Activation Mapping (Grad-CAM) - Visualizing CNN Decisions Using Grad-CAM for Explainable Image Classification</h3>
<p>https://colab.research.google.com/drive/1o0AilPAWzaSBxLBi-m0NcEtiJUTZFgtM#scrollTo=pOKI8fxzShp3&line=4&uniqifier=1</p>
<h3>Activity 3: Model Enhancement and
Performance Optimization | Improving CNN Performance Using Regularization, Fine-Tuning, and

Advanced Evaluation</h3>
<p>https://colab.research.google.com/drive/1o0AilPAWzaSBxLBi-m0NcEtiJUTZFgtM#scrollTo=bwGGGpfOaCXU&line=5&uniqifier=1</p>

<h1>Activity 1: Evaluation Metrics + Visualization</h1>
<h2>Precision, Recall, F1-Score</h2>
<img width="494" height="518" alt="image" src="https://github.com/user-attachments/assets/b6ef5dfb-a277-4621-b1fe-c0c08e6fd577" />
<h2>Confusion Matrix</h2>
<img width="842" height="731" alt="image" src="https://github.com/user-attachments/assets/63a6500d-b52b-46c8-90e7-4f69cf19ba96" />
<h2>Plot ROC Curve</h2>
<img width="787" height="647" alt="image" src="https://github.com/user-attachments/assets/caec393f-6c17-48f7-8b58-ecf1554f3e7c" />
<h2>Precision, Recall, F1 Visualization</h2>
<img width="1215" height="609" alt="image" src="https://github.com/user-attachments/assets/3f6eab7f-91f9-43f4-acd0-fd3e17449984" />

<h1>Activity 2: Model Interpretability using
Gradient-weighted Class Activation Mapping (Grad-CAM) - Visualizing CNN Decisions Using Grad-CAM for Explainable Image Classification</h1>
<h2>Grad-CAM Heatmap</h2>
<img width="497" height="493" alt="image" src="https://github.com/user-attachments/assets/cd90c4eb-0204-4828-a520-284bf10052a3" />
<h2>Grad-CAM Overlay</h2>
<img width="506" height="544" alt="image" src="https://github.com/user-attachments/assets/67afde8f-7442-4f33-b258-ef1cbf9f095d" />
<img width="412" height="419" alt="image" src="https://github.com/user-attachments/assets/f0878459-a6b9-414a-a61d-da109b5e6661" />
<h2>Interpret the Results</h2>
<p>The Grad-CAM visualization provides insight into how the model makes its predictions by highlighting the regions of the image that contribute most to the classification decision.

First, it can be observed that a significant portion of the heatmap is concentrated on the main object, which is the plant, particularly around the leaves. This indicates that the model is successfully identifying and focusing on the relevant features of the image. When the highlighted region corresponds to the correct object, it suggests that the model is learning properly and is able to extract meaningful patterns that are useful for classification.

However, it is also noticeable that some parts of the heatmap extend into the background and surrounding areas. This implies that the model is not exclusively focusing on the main object and is also considering irrelevant features during prediction. When the highlighted region includes the background, it indicates that the model is partially confused, as it is influenced by features that are not directly related to the object of interest.

Additionally, the heatmap appears somewhat scattered in certain areas, especially in the more detailed overlay visualization. This scattered pattern shows that the model’s attention is not fully concentrated and is instead distributed across multiple regions of the image. Such behavior suggests weak feature learning or imperfect localization, meaning the model has not yet developed a strong ability to precisely identify the most important features.

Overall, the results demonstrate that while the model is capable of recognizing the correct object and has learned relevant features, there is still room for improvement. The presence of background attention and scattered heatmap patterns indicates that the model could benefit from further training, improved dataset quality, or enhanced feature extraction techniques to achieve more accurate and focused predictions.</p>






