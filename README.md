# Network Traffic Analysis for Operating System Detection


## Table of Contents
- [Overview](#overview)
- [Problem Statement](#problem-statement)
- [Dataset](#dataset)
- [Features](#features)
- [Models](#models)
- [Model Evaluation](#model-evaluation)
- [Usage](#usage)
- [Installation](#installation)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgments](#acknowledgments)

## Overview

This is a comprehensive network traffic analysis project aimed at accurately detecting the operating system (OS) of devices based on their network traffic patterns. The work encompasses data preprocessing, feature engineering, model selection, and performance evaluation. 

## Problem Statement

The core objective of this project is to develop a robust and accurate method for identifying the operating systems (OS) used by devices through the analysis of network traffic. This capability is vital for enhancing cybersecurity, as it aids in intrusion detection and threat mitigation.

## Dataset

The project relies on a dataset containing a wide array of network traffic records. This dataset features a rich set of attributes, including detailed information on TCP and TLS protocols. Prior to model training, we conducted extensive data preprocessing to ensure data quality and consistency.

## Features

These features, including 'tcp.options.syn,' 'ip.ttl.syn,' 'tcp.window_size_value.syn,' 'ip.len.syn,' and 'tcp_flag_syn_ratio,' exhibit strong correlations with OS types. Their selection was facilitated by feature selection techniques, ensuring that our models are fed with the most relevant information.

## Models

The OS detection task is tackled using three distinct machine learning models:

1. **Random Forest**: Leveraging ensemble learning, the Random Forest model demonstrates robustness against noise and outliers. It handles both numerical and categorical features, making it an ideal choice for the dataset.

2. **Support Vector Machine (SVM)**: SVM is perfect model when dealing with high-dimensional data. It excels at discerning complex decision boundaries, which is essential for accurate OS detection based on network attributes.

3. **Gradient Boosting Machine (GBM)**: GBM harnesses the strength of multiple decision trees, uncovering patterns within the data. Its iterative nature allows it to capture nonlinear and complex relationships, an essential aspect of this OS detection problem.

## Model Evaluation

The models' performance is assessed using a battery of metrics, offering a holistic view of their effectiveness. The metrics include accuracy, precision, recall, and F1 score. These comprehensive measures ensure that the models' behavior is well-understood and evaluated from multiple angles.

## Usage

1. Clone this repository to your local machine.
2. Install the required Python libraries listed in `requirements.txt`.
3. Utilize the provided Jupyter notebooks for data preprocessing, feature selection, model training, and evaluation.

## Installation

To install the required dependencies, execute the following command:

```bash
pip install -r requirements.txt
```
## Contributing

Contributions are welcome! If you'd like to contribute to this project, please follow the standard GitHub workflow:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make your changes and test them.
4. Commit your changes and push them to your fork.
5. Create a pull request to merge your changes into the main repository.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
