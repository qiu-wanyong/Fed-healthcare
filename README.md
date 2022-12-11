# 2022FinTechathon 深圳国际金融科技大赛

团队：Fed-healthcare (联邦医疗)

面向智能体音感知的联邦学习系统-基于FATE平台

 ![](/figures/2022FinTechathon1.jpg)

# FederatedHealth_HeartSound
The horizontal FL (HFL) and vertical FL (VFL) paradigms for heart sound analysis.

#### Index Terms— Computer audition, federated learning, heart sound, information security, model interpretability

# Algorithm_Models

* Paradigms and workflows of horizontal and vertical federated learning (FL) on multi-institutional heart sound databases.

#### **Note:**  We first provide the final models and the relevant experimental results for this challenge. Other major program files will be uploaded after the paper of "Heart Sound Abnormality Detection from Multi-institutional Collaboration: Introducing a Federated Ensemble Learning Framework" is accepted.
 
 
## Results
 * Horizontally-Federated Learning vs Data-Centralised Learning
 
Table 1. A SUMMARY OF RESULTS (IN [%]) FOR CLASSIC XGBOOST AND THE  HFL MODEL WITH OPTIMAL PARAMETERS.

|            | Acc         | Se        |    Sp    |   UF1     |    UAR    |
| -----      | -----       | ----      |----      |----       |----       |
| XGBoost(Centralised Data)|  68.4       | 69.1      |67.6      | 68.4      |   68.4    |
| Homogeneous-SecureBoost  |  67.5     | 62.1     |72.8       | 67.4      |   67.5    |

Important parameters settings for the HFL and the XGBoost: tree depth=3,  tree number=30, subsample feature rate=1.0, learning rate=0.3.

 ![](/figures/HFL_matrix.jpg)
 
 Fig. 1. Normalised confusion matrix (in [%]) for the XGBoost and  Horizontal-SecureBoost models.
 
 
 Table 2. COMPARISON OF THE RESULTS (IN [%]) OF THE CONVENTIONAL  XGBOOST AND HETEROGENEOUS SECUREBOOST MODELS ON DATA  FOR EACH INSTITUTION.

|            |      XGBoost(Centralised Data)|      |Heterogeneous-SecureBoost|      |
|            | Acc       | Se      |    Sp   |  UAR    | Acc     | Se      |    Sp   |   UAR  |
| -----      | -----     | ----    |----     |----     |----     |-----    | ----    |----    |
| Db         |  86.7     |85.2     |88.3     |86.8     |82.7     |82.0     |83.5     |82.7    |
| Dc         |  86.7     |85.7     |87.5     |86.6     |93.3     |85.7     |92.0     |92.9    |
| Dd         |  93.3     |87.5     |92.0     |93.8     |96.2     |89.6     |96.4     |97.2    |
| De         |  88.2     |85.6     |86.7     |87.8     |87.6     |82.6     |86.3     |84.3    |
| Df         |  86.8     |90.9     |81.3     |86.1     |79.5     |75.5     |71.3     |78.4    |

![](/figures/VFL_matrix.jpg)
 
Fig. 2. Normalised confusion matrix (in [%]) for XGBoost and Vertically-  SecureBoost models trained at D_e database.

## Awards
  
 ![](/figures/Awards1.png)
 ![](/figures/Awards2.png)
 
 Fig. 3. 2022Fintechathon Shenzhen International Fintech Competition First Prize.

 
## Availability

1. Voice of the Body (VoB) 是第一个计算机听觉医学数据库平台，用于对体音信号进行分析. https://www.vob-bit.org/

2. Classification of Heart Sound Recordings (PhysioNet/CinC challenge): https://physionet.org/content/challenge-2016/1.0.0.

3. SHAP (SHapley Additive exPlanations) is a game-theoretic method to explain the output of ML models. https://shap.readthedocs.io.

4. FATE (Federated AI Technology Enabler) supports the FL architecture, as well as the secure computation and development of various ML algorithms. https://github.com/FederatedAI/FATE.


## Cite As
Wanyong Qiu, Chen Quan, Lixian Zhu, Yongzi Yu, Zhihua Wang, Yu Ma, Mengkai Sun, Yi Chang, Kun Qian*, Bin Hu∗, Yoshiharu Yamamoto and Bjoern W. Schuller, “Heart Sound Abnormality Detection from Multi-institutional Collaboration: Introducing a Federated Ensemble Learning Framework”, JBHI, pp. 1-11, Submitted, October 2022.


