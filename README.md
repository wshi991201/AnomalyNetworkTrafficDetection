# Anomaly Network Traffic Detection

## Introduction/Background:
Due to nowadays' ever-growing network security concerns, an accurate and efficient way to distinguish normal activity flows from cyber attacks becomes exceedingly important. Our project will develop a trained machine in place of Intrusion Detection Systems (IDS) to monitor network traffic for suspicious activities. To decrease false alarms in IDS, we plan to investigate and contrast the influences of more than 80 features branched under some of the most common types of attacks – web-based, brute force, DoS (disk operating system), DDoS (distributed denial of service), infiltration, heart-bleed, bots, and portscan. Such a model would strengthen available defense tools against those sophisticated network attacks and alleviate burdens of website owners and administrators.

## Problem Definition:
We aim to build an IDS model to distinguish benign and potential anomaly network traffic. The goal is to minimize false positives while not permitting false negatives, or the most serious states of identifying malicious activity as acceptable.
  
## Methods:
We plan to apply both unsupervised and supervised methodologies in analyzing the datasets. For unsupervised learning, K-means algorithm will be utilized to cluster different network activities based on distinct features. For supervised learning, we will construct regression models for different labels of attack types and normal activity. Scikit-learning provides well-implemented algorithms for regression, model selection, and etc. Therefore, we will use existing packages and libraries in Scikit-learning for convenience. Also, in order to extract the aforementioned 80 network traffic features from the dataset, we will use python package CICFlowMeter, which is a flow-based feature extractor and outputs the given pcap format file.
The following step is to split and feed our data to the predefined model, and for a 5-day network flow, we will use the first three days for training and the last two days for testing.

## Dataset:
- [Intrusion Detection Evaluation Dataset (CIC-IDS2017)](https://www.unb.ca/cic/datasets/ids-2017.html)
- Labeled network flows, including full packet payloads in pcap format and CSV files for machine/deep learning purposes
- Covered ten criteria as a reliable dataset: complete network configuration, complete traffic, labeled dataset, complete interaction, complete capture, available protocols, attack diversity, heterogeneity, feature set, and MetaData
- Started at 9am on Monday, July 3, 2017 until 5pm on Friday July 7, 2017, for a total of 5 days

## Potential Results and Discussion:
We expect high accuracy of identifying malicious traffic in both supervised and unsupervised learning. However, the normal traffic flows could be hard to accurately recognize because we prioritize training in attack features to avoid false negatives. To evaluate our machine learning algorithms, we will use a confusion matrix to easily extract false positives and false negatives proportions and to compute precision, recall, and accuracy of our model.

## Proposed Timeline:
- Project Proposal:
  - Dataset, reference, and target problem (Yijie Gong, Wangzhuo Shi) - June 6th
  - Proposal first draft and review (Feng Gao, Heeyong Huang) - June 10th
  - 2-min presentation video (Zhenyu Chen) - June 13th
- Midterm Report
  - Dataset cleaning and feature selection (Yijie Gong) - June 22nd
  - Supervised and unsupervised methods implementation (Feng Gao, Wangzhuo Shi) - June 29th
  - Report first draft and model evaluation (Heeyong Huang, Zhenyu Chen) - July 4th
  - Mid-term report final draft (Team) - July 6th
- Final Report
  - Parameter, code, and model optimization (Feng Gao, Yijie Gong) - July 13th
  - Project final draft (Heeyong Huang, Wangzhuo Shi) - July 25th
  - Final team video (Team) - July 29th


## References:
- [Sharafaldin, I., Habibi Lashkari, A., & Ghorbani, A. A. (2018). Toward Generating a New Intrusion Detection Dataset and Intrusion Traffic Characterization. In Proceedings of the 4th International Conference on Information Systems Security and Privacy. 4th International Conference on Information Systems Security and Privacy. SCITEPRESS - Science and Technology Publications.](https://doi.org/10.5220/0006639801080116)
- [Erman, J., Arlitt, M., & Mahanti, A. (2006). Traffic classification using clustering algorithms. In Proceedings of the 2006 SIGCOMM workshop on Mining network data - MineNet ’06. the 2006 SIGCOMM workshop. ACM Press.](https://doi.org/10.1145/1162678.1162679)
- [Disha, R. A., & Waheed, S. (2022). Performance analysis of machine learning models for intrusion detection system using Gini Impurity-based Weighted Random Forest (GIWRF) feature selection technique. In Cybersecurity (Vol. 5, Issue 1). Springer Science and Business Media LLC.](https://doi.org/10.1186/s42400-021-00103-8)
- [Chitrakar, R., & Huang, C. (2012). Anomaly Based Intrusion Detection Using Hybrid Learning Approach of Combining k-Medoids Clustering and Naïve Bayes Classification. In 2012 8th International Conference on Wireless Communications, Networking and Mobile Computing. 2012 8th International Conference on Wireless Communications, Networking and Mobile Computing (WiCOM 2012). IEEE.](https://doi.org/10.1109/wicom.2012.6478433)















Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [Basic writing and formatting syntax](https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/wshi991201/wshi991201.github.io/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.
