# IoT Threat Classification with Ensemble Machine Learning Models

![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)
![GitHub Stars](https://img.shields.io/github/stars/jorgesandoval/iotthreat-classification-ensemble.svg)
![GitHub Downloads](https://img.shields.io/github/downloads/jorgesandoval/iotthreat-classification-ensemble/total.svg)
![GitHub Forks](https://img.shields.io/github/forks/jorgesandoval/iotthreat-classification-ensemble.svg)


![Alt text](images/IoTThreat.png)
This repository houses a Jupyter notebook for IoT threat detection using ensemble machine learning.

![Alt text](image.png)

## 📖 Table of Contents
- [IoT Threat Classification with Ensemble Machine Learning Models](#iot-threat-classification-with-ensemble-machine-learning-models)
  - [📖 Table of Contents](#-table-of-contents)
  - [📌 Overview](#-overview)
  - [📊 Dataset](#-dataset)
  - [🔧 Dependencies](#-dependencies)
  - [🚀 Usage](#-usage)
  - [📈 Key Findings](#-key-findings)
  - [💡 Contributions](#-contributions)
  - [📜 License](#-license)
  - [👤 Authors](#-authors)
  - [🙌 Acknowledgements](#-acknowledgements)

## 📌 Overview
The notebook explores the application of various machine learning models to the domain of IoT security, with a focus on threat classification. It culminates in the creation of an ensemble model that integrates the predictions of multiple models to enhance accuracy and reliability. The performance of each model is meticulously measured using accuracy, precision, and recall metrics, and the results are compared to identify the most effective approach.

## 📊 Dataset

* **File Name**: `iot_threat_data.csv`
* **Description**: The dataset comprises features extracted from network traffic, indicative of potential IoT threats. It undergoes preprocessing to handle missing values and is then used for feature selection and model training.

## 🔧 Dependencies

To run the notebook, you'll need the following libraries:

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

You can install these using `pip`:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## 🚀 Usage

1. **Clone the repository:**

   ```bash
   git clone https://github.com/yourusername/iot-threat-classification-ensemble.git
   ```
2. **Navigate to the cloned directory and open the Jupyter notebook"**

    ```bash
        cd iot-threat-classification-ensemble
        jupyter notebook
    ```
3. **Run the notebook**: Execute the notebook cells sequentially to preprocess the data, train the XGBoost model, and evaluate its performance.
## 📈 Key Findings

* **Ensemble Model**: Achieved an accuracy of approximately 88.43%, with a precision score slightly higher than its accuracy, indicating that the model's predictions are quite reliable.
* **K-Nearest Neighbors (KNN)**: Exhibited nearly equivalent accuracy to the ensemble model, with notably higher precision, suggesting a high percentage of correct positive predictions.
* **Neural Network**: Ranked third in accuracy, but with a lower precision compared to its accuracy, indicating potential over-prediction in certain classes.
* **Gradient Boosting**: Showcased the highest precision among the top models, although with slightly lower accuracy than the Neural Network, suggesting very reliable positive predictions.
* **Random Forest & Extra Trees**: Both models demonstrated almost identical accuracy and precision scores, performing well in accuracy but with room for improvement in precision.
* **Decision Tree**: Performed on par with the Random Forest and Extra Trees models, as expected due to the nature of Random Forests being ensembles of Decision Trees.
* **Logistic Regression & SVM**: These models had similar accuracy scores but lower precision than the top-performing models, indicating a higher number of false positive predictions.
* **Gaussian Naive Bayes**: Despite ranking last in accuracy, it had a high precision score, nearly matching that of the Gradient Boosting model, suggesting that its positive predictions are highly reliable.

The ensemble approach demonstrated the benefit of combining multiple models to improve prediction reliability and accuracy, outperforming individual models in overall metrics.

## 💡 Contributions

Contributions to this repository are very welcome! Whether it's fixing bugs, improving the documentation, adding new features, or providing feedback, your insights can help improve this project. Here's how you can contribute:

1. **Fork the Project**
* Navigate to the main page of the repository.
* Click on the Fork button on the top right.

2. **Create Your Feature Branch**
    ```bash
    git checkout -b feature/AmazingFeature
    ```

3. **Commit Your Changes**
    ```bash
    git commit -m 'Add some AmazingFeature'
    ```
4. **Push to the Branch**
    ```bash
    git push origin feature/AmazingFeature
    ```
5. **Open a Pull Request**
* Navigate back to the main page of your forked repository.
* Click on the "Pull requests" tab.
* Click on the green "New pull request" button.


## 📜 License

Distributed under the MIT License. See [LICENSE](https://opensource.org/licenses/MIT) for more information.

## 👤 Authors
* [Jorge Sandoval](https://www.linkedin.com/in/jorge-g-sandoval/)

## 🙌 Acknowledgements

I would like to express my sincere appreciation to the Canadian Institute for Cybersecurity (CIC) for their pivotal role in the advancement of IoT security research through the provision of the CIC IoT Dataset 2023. This dataset has been a crucial asset in my research, offering a robust benchmark for large-scale attacks in IoT environments.

The CIC IoT Dataset 2023 is a product of the CIC's commitment and expertise, featuring a detailed topology with numerous real IoT devices acting in both offensive and defensive capacities. The dataset includes 33 meticulously documented attacks across seven categories, providing a rich foundation for the development of advanced security analytics applications.

Key contributions of the CIC IoT Dataset 2023 that have been particularly beneficial include:

- A novel and realistic IoT attack dataset, utilizing a comprehensive network of real IoT devices.
- Comprehensive documentation and data for 33 distinct attacks, classified into seven categories, showcasing their potential for replication.
- Assessments of various machine and deep learning algorithms using the dataset to effectively classify and detect IoT network traffic as either malicious or benign.

The CIC's dedication to enhancing IoT security research is commendable, and their willingness to share this dataset underscores their commitment to the cause. It stands as a vital resource for numerous initiatives aimed at improving different facets of IoT security.

For further details about the CIC IoT Dataset 2023 and to access the data, please visit the [dataset page](https://www.unb.ca/cic/datasets/iotdataset-2023.html). The dataset is available for download at [this link](http://205.174.165.80/IOTDataset/CIC_IOT_Dataset2023/).

My gratitude towards the CIC for their support and for equipping the research community with such a valuable resource is immense.





