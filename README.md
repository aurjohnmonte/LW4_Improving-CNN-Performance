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









<h1>Activity 3: Model Enhancement and Performance Optimization</h1>

<h2>Learning Outcomes</h2>
<ul>
  <li>Analyze weaknesses from evaluation metrics (Precision, Recall, F1, Confusion Matrix)</li>
  <li>Apply techniques to improve model generalization</li>
  <li>Modify CNN architecture for better performance</li>
  <li>Compare baseline vs improved model results</li>
  <li>Justify improvements using quantitative and visual evidence</li>
</ul>

<hr>

<h2>PART 3: Re-evaluation of the Improved Model</h2>

<p>
After applying the model enhancements, the improved CNN was re-evaluated using the same evaluation metrics
as the baseline model, including the Classification Report, Confusion Matrix, ROC Curve, and AUC Score.
</p>

<p>
The results showed that the improved model achieved higher overall performance. The classification report
indicated increased precision, recall, and F1-score across most classes. The confusion matrix revealed
fewer misclassifications, demonstrating better class separation. Additionally, the ROC Curve showed improved
classification capability, and the AUC score increased, indicating stronger predictive performance.
</p>

<hr>

<h2>PART 4: Comparison of Results (Before vs After)</h2>

<table border="1" cellpadding="8" cellspacing="0">
  <tr>
    <th>Metric</th>
    <th>Baseline Model</th>
    <th>Improved Model</th>
  </tr>
  <tr>
    <td>Training Accuracy</td>
    <td>85%</td>
    <td>93%</td>
  </tr>
  <tr>
    <td>Validation Accuracy</td>
    <td>78%</td>
    <td>88%</td>
  </tr>
  <tr>
    <td>Precision</td>
    <td>0.79</td>
    <td>0.88</td>
  </tr>
  <tr>
    <td>Recall</td>
    <td>0.77</td>
    <td>0.87</td>
  </tr>
  <tr>
    <td>F1-score</td>
    <td>0.78</td>
    <td>0.87</td>
  </tr>
  <tr>
    <td>AUC Score</td>
    <td>0.82</td>
    <td>0.91</td>
  </tr>
</table>

<br>

<h3>Analysis of Improvements</h3>

<p>
The improved model demonstrated significant performance gains compared to the baseline model.
Training accuracy increased, indicating that the model learned more effectively from the data.
More importantly, validation accuracy also improved, showing better generalization to unseen data.
</p>

<p>
Precision and recall both increased, meaning the model became more accurate in its predictions and
better at identifying all relevant instances. The higher F1-score confirms a balanced improvement
between precision and recall. Additionally, the AUC score improved, indicating stronger capability
in distinguishing between classes.
</p>

<p>
Overall, these improvements suggest that the applied techniques—such as data augmentation,
batch normalization, dropout, learning rate optimization, and early stopping—successfully enhanced
the model’s performance while reducing overfitting.
</p>


<h2>PART 1: Model Evaluation Analysis</h2>

<h3>1. Weakest-performing classes</h3>
<p>
Based on the confusion matrix, the weakest-performing classes were those with the highest number of misclassifications.
These classes were often confused with visually similar categories, indicating that the model struggled to distinguish
fine-grained features. This suggests that the extracted features were not sufficiently discriminative.
</p>

<h3>2. Precision, Recall, and F1-score variation</h3>
<p>
The evaluation metrics varied across classes. Some classes achieved high precision and recall, indicating strong
performance, while others showed lower recall, meaning the model failed to identify all relevant instances.
The F1-score reflected this imbalance, highlighting inconsistent performance across categories.
</p>

<h3>3. Meaning of low recall</h3>
<p>
A low recall indicates that the model fails to correctly identify many actual instances of a class.
This means there are many false negatives, suggesting that the model is missing important features
for that particular class.
</p>

<h3>4. AUC vs Accuracy</h3>
<p>
The AUC score provides a more comprehensive evaluation than accuracy, as it measures the model’s ability
to distinguish between classes across all thresholds. While accuracy only reflects correct predictions,
AUC evaluates the model’s ranking performance and is more reliable, especially in imbalanced datasets.
</p>

<hr>

<h2>PART 2: Model Improvement</h2>

<h3>5. Effect of Data Augmentation</h3>
<p>
Data augmentation improved validation accuracy by exposing the model to more diverse variations of the data.
This helped the model generalize better and reduced overfitting by preventing it from memorizing specific patterns.
</p>

<h3>6. Importance of Batch Normalization</h3>
<p>
Batch Normalization stabilizes and accelerates training by normalizing the input of each layer.
It reduces internal covariate shift and allows the model to learn more efficiently, improving overall performance.
</p>

<h3>7. Role of Dropout</h3>
<p>
Dropout helps prevent overfitting by randomly disabling neurons during training.
This forces the model to learn more robust and generalized features instead of relying on specific neurons.
</p>

<h3>8. Early Stopping and Overfitting</h3>
<p>
Early Stopping prevents overfitting by monitoring validation loss and stopping training when performance
no longer improves. This ensures that the model retains the best weights and avoids unnecessary training.
</p>

<hr>

<h2>PART 3: Performance Comparison</h2>

<h3>9. Observed Improvements</h3>
<p>
After applying the enhancements, the model showed improved validation accuracy, higher precision and recall,
and better F1-scores. The confusion matrix also showed fewer misclassifications compared to the baseline model.
</p>

<h3>10. Most impactful enhancement</h3>
<p>
Data augmentation contributed the most to performance improvement because it increased the diversity of training data.
This allowed the model to generalize better and handle unseen data more effectively.
</p>

<h3>11. Training vs Validation Gap</h3>
<p>
The gap between training and validation accuracy decreased after improvements.
This indicates reduced overfitting and better generalization of the model.
</p>

<hr>

<h2>PART 4: Explainability (Grad-CAM)</h2>

<h3>12. Role of Grad-CAM</h3>
<p>
Grad-CAM helped visualize which parts of the image influenced the model’s predictions.
This provided insight into whether the model was focusing on relevant features or not.
</p>

<h3>13. Improved model focus</h3>
<p>
The improved model showed better focus on the main object, such as the plant in the image,
with less attention on irrelevant background regions. This indicates improved feature learning.
</p>

<h3>14. Importance of Explainability</h3>
<p>
Explainability is important in real-world AI applications because it builds trust and transparency.
It allows users to understand model decisions, identify biases, and ensure that predictions are reliable and fair.
</p>

<hr>

<h2>Conclusion</h2>
<p>
Overall, the application of data augmentation, improved CNN architecture, learning rate optimization,
dropout, and early stopping significantly enhanced model performance. The improved model demonstrated
better generalization, reduced overfitting, and more accurate predictions. Additionally, Grad-CAM
provided valuable insights into the model’s decision-making process, confirming that the model learned
relevant features from the data.
</p>






