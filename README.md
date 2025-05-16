# Securing-Internet-of-Things-devices-using-CIC-IoT-Net-Flow-Dataset

The rise of Internet of Things (IoT) has made the digital landscape transformed into providing more services but also introduced significant cybersecurity challenges by expanding potential vulnerabilities. Security systems such as Data Loss Prevention (DLP), Intrusion Detection Systems (IDS) and firewalls are struggling to keep up with these modern threats. They often produce a high number of false positives and lack the capability to identify more advanced, evolving attacks. To address these shortcomings, our research presents a machine learning models where we compare the ML models and analyse in detail as to which model produces the best accuracy. This approach has been documented each model and made sure the results are best for the networks for processing sequential data. The hybrid design improves detection accuracy and reduces the rate of false positives.
Furthermore, we developed these machine learning models are two datasets in order to figure out the best results. The novelty of this research lies in the hyper parameter tuning of machine learning models to achieve best results. The main contributions of this research are the extensive machine learning and deep learning algorithms for detecting and classifying malicious traffic. Our research conducted five novel machine learning models on UQ-NIDS dataset and added hyper parameter tuning in order to determine how well the model performs on those IoT attacks and for CICIoT dataset, our research is performed extensively on the classification of attack categories and implemented three novel algorithms to find the best model for each attack categories. And our research was able to find that Random Forest and Logistic Regression performs well on both the datasets and also identifying different categories in IoT attacks


## Dataset Description
The CICIoT dataset contains over 548 GB of raw network traffic data which are stored in PCAP format using Wireshark. In order to make this dataset usable for machine learning 47 key features are extracted from the raw data. This dataset is available in two formats, the original PCAP files for advanced analysis and CSV files which contains extracted features for machine learning tasks. Malicious traffic has 33 different attack types which are categorized into 7 primary groups. There is a total of 46,686,579 records. DDoS category contains 33,984,560 records, DoS category comprises of 8,090,738 records which focuses on single source attacks which can disrupt the services availability. PSHACK flood comprises of 4,094,755, HTTP flood comprises of 28,790 records. SYN flood comprises of 2,028,834 records. The spoofing category has 486,504 records. And Mirai Botnet category consists of 2,634,124 records, Benign Traffic has 1,098,195 records. This comprehensive breakdown shows the diversity of CIC IoT dataset which makes it an invaluable resource for developing IoT intrusion detection systems.

## Feature Extraction
The dataset was divided into 80% training data and 20% testing data. This split makes sure that training split provides suffucicient data diversity for the machine learning model to learn paatern effectively while the testing set provides enough representation of unseen data to evaluate the generalization capabilitiesof the trained models. 
All features were normalized using Standard Scaler method and this method ensures uniform range to improve performanceand convergence of machine learningduring training. The data split facilitated three classification tasks:
Binary classification: which distinguished between malicious and benign traffic.
Grouped classification: which categorized traffic into seven attack groups such as DDoS, DoS and reconnaissance.
Multiclass classification: which classified traffic into 33 individual attack types.

## Evaluation
The evaluation process for the CICIoT dataset involves structured pipeline to assess the performance of various machine learning mthods for detecting and classifying the malicious IoT network traffic. The main focus is on the three levels of classification: binary (benign and malicious), grouped (7 attack category), multiclass (34 individual attacks). The dataset is initially combined, shuffled and divided into training and testing subsets. The features are then normalized using standardscaler to make sure consistent scaling. The evaluation highlighted the robustness. On the CICIoT dataset the feasibility of multiclass classification at 34-class, 8- class, and 2-class levels was established, with Decision Tree consistently delivering the best results across tasks. This research also provided impactful insights and confirming that hyperparameter tuning and tailored the dataset specific preprocessing significantly to enhance model performance. And ensemble methods like Random Forest and XGBoost proved their robust for IoT anomaly detection. 

### Based on Accuracy
The CICIoT dataset took about 12 hours to completely execute the program as they more that 12 GB of storage which the system had to handle. And for the CICIoT dataset, the classification plays a vital role. And for 32 class classification (33+1), the accuracy is highest for Decision Tree (99.19%) and Support Vector Machine (78.17%) has the lowest accuracy.

For the 8 class classification of the CICIoT dataset, the highest accuracy is achieved by Decision Tree (99.40%) and the lowest accuracy for the 8 class classification belongs to Support Vector Machine model (82.30%).

The 2 (1+1) class classification of the CICIoT dataset. Decision Tree (99.58%) holds the highest accuracy and Support Vector Machine (98.71%) has the lowest accuracy.
Decision Tree consistently outperformed other models in various classification tasks and achieves the highest accuracy across 32, 8 and 2 class classification.
Support Vector Machine generally had lower accuracy which indicates it may not be the suitable model for this classification tasks.

### Based on Precision
For CICIoT dataset, the classification is divided into 3 categories. 34 (33+1) class classification based on the attack categories. The highest precision is achieved by Random Forest (96.55%) and the lowest achieved model is Support Vector Machine (52.86%).

For the 8 class classification of the CICIoT dataset, the highest precision is achieved by Decision Tree (99.40%) and the lowest precision  for the 8 class classification belongs to Support Vector Machine model (82.30%).

For the 2 (1+1) class classification of the CICIoT dataset, the highest precision is achieved by Decision Tree (99.40%) and the lowest precision for the 8 class classification belongs to Support Vector Machine model (82.30%).

### Based on Recall
For CICIoT dataset, the classification is divided into 3 categories. 34 (33+1) class classification based on the attack categories. The highest recall is achieved by Random Forest (96.44%) and the lowest recall achieved model is Support Vector Machine (42%).

For the 8-class classification of the CICIoT dataset, the highest precision is achieved by Decision Tree (99.40%) and the lowest precision for the 8 class classification belongs to Support Vector Machine model (82.30%).

For the 2 (1+1) class classification of the CICIoT dataset, the highest precision is achieved by Decision Tree (99.40%) and the lowest precision for the 8 class classification belongs to Support Vector Machine model (82.30%).

### Based on F1 Score
For CICIoT dataset, the classification is divided into 3 categories. 34 (33+1) class classification based on the attack categories. The highest recall is achieved by Random Forest (96.44%) and the lowest recall achieved model is Support Vector Machine (43.3722%).

For the 8-class classification of the CICIoT dataset, the highest precision is achieved by Decision Tree (99.40%) and the lowest precision for the 8 class classification belongs to Support Vector Machine model (82.30%).

For the 2 (1+1) class classification of the CICIoT dataset, the highest precision is achieved by Decision Tree (99.40%) and the lowest precision for the 8-class classification belongs to Support Vector Machine model (82.30%).

## Discussion
The Decision Tree , models achieved higher accuracies respectively. The research results highlights the importance of feature selection for training the model, indicating Decision Tree and Logistic Regression is a reliable choice for 34 class. 
For 8 class classification Decision Tree and Random Forest are the two best models followed by Logistic Regression and Support Vector Machine.
For 2 class classification, once again Decision Tree outperformed the other models.  This emphasizes the significance of considering machine learning models for complex classification tasks as they improve the overall performance over traditional approaches


