# Privacy-preserving Machine Learning: Resources and Materials

# Table of Contents
1. [About](#about)
2. [Survey Papers](#survey-papers)
3. [Cryptographic-based Approaches](#cryptographic-based-approach)
4. [Non-cryptographic-based Approaches](#non-cryptographic-based-approaches)
5. [Courses](#courses)
6. [Frameworks](#frameworks)
7. [Other Resources](#other-resources)

# About  
This is a compiled list of resources and materials for PPML.  

## Survey Papers

1. [Arxiv’20] [Privacy in Deep Learning: A Survey](https://www.researchgate.net/publication/340963602_Privacy_in_Deep_Learning_A_Survey)
2. [Arxiv’20] [SoK: Training Machine Learning Models over Multiple Sources with Privacy Preservation](https://arxiv.org/abs/2012.03386)
3. [IEEEAccess’20] [Privacy-Preserving Deep Learning on Machine Learning as a Service: A Comprehensive Survey](https://ieeexplore.ieee.org/document/9194237)
4. [PETS’21] [SoK: Privacy-Preserving Computation Techniques for Deep Learning](https://petsymposium.org/2021/files/papers/issue4/popets-2021-0064.pdf)
5. [PETS’21] [SoK: Efficient Privacy Preserving Clustering](https://eprint.iacr.org/2021/809)

# Cryptographic-based Approach

## Training Phase
### Homomorphic Encryption (HE) & Functional Encryption (FE)

1. [BMC medical genomics’18] [Privacy-preserving logistic regression training](https://bmcmedgenomics.biomedcentral.com/articles/10.1186/s12920-018-0398-y)
2. [Arxiv’19] [CryptoNN: Training Neural Networks over Encrypted Data](https://arxiv.org/abs/1904.07303) (Functional Encryption). [Code](https://github.com/iRxyzzz/nn-emd) (Python)
3. [PETS’18] [CryptoDL: Privacy-preserving Machine Learning as a Service](https://petsymposium.org/2018/files/papers/issue3/popets-2018-0024.pdf) 
4. [*IEEE/CVF’19*] [Towards Deep Neural Network Training on Encrypted Data](https://openaccess.thecvf.com/content_CVPRW_2019/papers/CV-COPS/Nandakumar_Towards_Deep_Neural_Network_Training_on_Encrypted_Data_CVPRW_2019_paper.pdf)
5. [ArXiv’20] [Neural Network Training With Homomorphic Encryption](https://arxiv.org/abs/2012.13552)
6. [ArXiv’20] [PrivFT: Private and Fast Text Classification with Homomorphic Encryption](https://arxiv.org/abs/1908.06972?utm_source=feedburner&utm_medium=feed&utm_campaign=Feed%253A+arxiv%252FQSXk+%2528ExcitingAds%2521+cs+updates+on+arXiv.org%2529)

**HE-based Hybrid Techniques**

1. [NeurlPS’20] [Glyph: Fast and Accurately Training Deep Neural Networks on Encrypted Data](https://arxiv.org/pdf/1911.07101.pdf) (Switch between HE schemes: TFHE and BGV)
2. [NDSS’21] [POSEIDON: Privacy-Preserving Federated Neural Network Learning](https://arxiv.org/abs/2009.00349) (Federated Learning + HE) (Code is confidential)

### Secure Multi-Party Computation (SMPC)

1. [S&P’17] [SecureML: A System for Scalable Privacy-Preserving Machine Learning](https://eprint.iacr.org/2017/396). [Code](https://github.com/shreya-28/Secure-ML) (C++)
2. [CCS’19] [QUOTIENT: two-party secure neural network training and prediction](https://dl.acm.org/citation.cfm?id=3339819)
3. [Arxiv’19] [CodedPrivateML: A Fast and Privacy-Preserving Framework for Distributed Machine Learning](https://arxiv.org/abs/1902.00641)
4. [PETS’20] [Falcon: Honest-Majority Maliciously Secure Framework for Private Deep Learning](https://arxiv.org/abs/2004.02229). [Code](https://github.com/snwagh/falcon-public) (C++)
5. [ICPP’20] [ParSecureML: An Efficient Parallel Secure Machine Learning Framework on GPUs](https://dl.acm.org/doi/pdf/10.1145/3404397.3404399). [Code](https://github.com/ZhengChenCS/ParSecureML) (C++)
6. [PoPETs’20] [FLASH: Fast and Robust Framework for Privacy-preserving Machine Learning](https://eprint.iacr.org/2019/1365).
7. [NDSS’20] [BLAZE: Blazing Fast Privacy-Preserving Machine Learning](https://eprint.iacr.org/2020/042)
8. [USENIX’21] [Cerebro: A Platform for Multi-Party Cryptographic Collaborative Learning](https://www.usenix.org/conference/usenixsecurity21/presentation/zheng). [Code](https://github.com/mc2-project/cerebro) (Python)
9. [USENIX’21] [Fantastic Four: Honest-Majority Four-Party Secure Computation With Malicious Security](https://www.usenix.org/system/files/sec21fall-dalskov.pdf). [Code](https://github.com/csiro-mlai/mnist-mpc/tree/v1) (Python)
10. [S&P’21] [CryptGPU: Fast Privacy-Preserving Machine Learning on the GPU](http://arxiv.org/abs/2104.10949). [Code](https://github.com/jeffreysijuntan/CryptGPU) (Python)
11. [USENIX 2021] [SWIFT: Super-fast and Robust Privacy-Preserving Machine Learning](https://www.semanticscholar.org/paper/SWIFT%3A-Super-fast-and-Robust-Privacy-Preserving-Koti-Pancholi/55e9017bcf4ffec2d34c760cc832d72e39c73216)
12. [Arxiv’21] [Adam in Private: Secure and Fast Training of Deep Neural Networks with Adaptive Moment Estimation](https://arxiv.org/abs/2106.02203)
13. [Arxiv’21] [Secure Quantized Training for Deep Learning](https://arxiv.org/abs/2107.00501). [Code](https://github.com/csiro-mlai/mnist-mpc/tree/master) (Python)
14. [ACMCCS’21] *[ABY2.0: Improved Mixed-Protocol Secure Two-Party Computation.](https://www.usenix.org/system/files/sec21summer_patra.pdf)* [Code](https://github.com/encryptogroup/MOTION2NX) (C++)

**SMPC-based Hybrid Techniques**

1. [CCS’18] [ABY3: A Mixed Protocol Framework for Machine Learning](https://eprint.iacr.org/2018/403.pdf). [Code](https://github.com/ladnir/aby3) (C++)
2. [PETS’18] [SecureNN: 3-Party Secure Computation for Neural Network Training](https://eprint.iacr.org/2018/442.pdf). [Code](https://github.com/snwagh/securenn-public) (C++)
3. [NDSS’20] [Trident: Efficient 4PC Framework for Privacy Preserving Machine Learning](https://eprint.iacr.org/2019/1315)
4. [Arxiv’21] [Tetrad: Actively Secure 4PC for Secure Training and Inference](https://arxiv.org/abs/2106.02850)
5. [S&P’21] [MPCLeague: Robust 4-party Computation for Privacy-preserving Machine Learning](https://dp-ml.github.io/2021-workshop-ICLR/files/9.pdf)

### Hybrid Techniques

1. [IACR Cryptol’17] [Private Collaborative Neural Network Learning](https://eprint.iacr.org/2017/762.pdf) (SMPC + DP)

## Inference Phase

### Homomorphic Encryption (HE) & Functional Encryption

1. [ICML’16] [CryptoNets: Applying Neural Networks to Encrypted Data with High Throughput and Accuracy](https://proceedings.mlr.press/v48/gilad-bachrach16.html). [Code](https://github.com/microsoft/CryptoNets) (C#).

### Secure Multi-Party Computation (SMPC)

1. [SIGSAC’17] [Oblivious Neural Network Predictions via MiniONN Transformations](https://eprint.iacr.org/2017/452.pdf). [Code](https://github.com/SSGAalto/minionn) (Python).
2. [ASIACCS’18] [Chameleon: A Hybrid Secure Computation Framework for Machine Learning Applications](https://arxiv.org/abs/1801.03239)
3. [S&P’20] [CrypTFlow: Secure TensorFlow Inference](https://www.microsoft.com/en-us/research/publication/cryptflow-secure-tensorflow-inference/)

# Non-cryptographic-based Approaches

## Federated Learning
- [AISTATS'17] [Communication-Efficient Learning of Deep Networks from Decentralized Data (FedAvg)](https://arxiv.org/pdf/1602.05629.pdf)

### Federated Learning on Non-public Datasets
Works that do experiments on non-public / private datasets
- [RadiotherapyAndOncology'16] [Distributed learning: developing a predictive model based on data from multiple hospitals without data leaving the hospital–a real life proof of concept](https://www.sciencedirect.com/science/article/pii/S0167814016343365)
- [Nature'21] [End-to-end privacy preserving deep learning on multi-institutional medical imaging](https://www.nature.com/articles/s42256-021-00337-8) - [Code](https://github.com/gkaissis/PriMIA)
- [JMIR Medical Informatics'21] [Federated Learning of Electronic Health Records to Improve Mortality Prediction in Hospitalized Patients With COVID-19: Machine Learning Approach](https://medinform.jmir.org/2021/1/e24207/)
- [Nature'22] [Federated deep learning for detecting COVID-19 lung abnormalities in CT: a privacy-preserving multinational validation study](https://www.nature.com/articles/s41746-021-00431-6)
- [Nature'22] [Federated learning enables big data for rare cancer boundary detection](https://www.nature.com/articles/s41467-022-33407-5)
- [Genome Biology'22] [sPLINK: a hybrid federated tool as a robust alternative to meta-analysis in genome-wide association studies](https://link.springer.com/article/10.1186/s13059-021-02562-1)
- [SPML'22] [Federated Learning for Privacy-Preserving Medical Data Sharing in Drug Development](https://www.ewadirect.com/proceedings/ace/article/view/17879)
- [ICMHI'24] [Federated Learning and Differential Privacy Techniques on Multi-hospital Population-scale Electrocardiogram Data](https://dl.acm.org/doi/10.1145/3673971.3673990)
- [eBioMedicine'24] [Decentralised, collaborative, and privacy-preserving machine learning for multi-hospital data](https://www.sciencedirect.com/science/article/pii/S2352396424000410) - [Code](https://github.com/cleverhans-lab/DeCaPH)
- [Nature'25] [Privacy-preserving federated learning for collaborative medical data mining in multi-institutional settings](https://www.nature.com/articles/s41598-025-97565-4)

# Courses
- [Private AI Series](https://courses.openmined.org/courses) (OpenMined)
- [MIT 6.875: Foundations of Cryptography](https://mit6875.github.io/)  (MIT, Fall 2021)  - [Lecture Notes](https://khoaduynguyen.com/tags/mit6-875/)
- [Privacy in Statistics and Machine Learning](https://dpcourse.github.io/schedule.html) (Boston University, Spring 2021)
- [Algorithms for Private Data Analysis - Fall 2020](http://www.gautamkamath.com/CS860-fa2020.html) (University of Waterloo, Fall 2020)
- [Privacy Preserving Machine Learning](http://researchers.lille.inria.fr/abellet/teaching/private_machine_learning_course.html) (University of Lille, 2021) 

# Frameworks
- [PySyft (Python)](https://github.com/OpenMined/PySyft): decouples private data from model training (using FL, DP, HE, SMPC...) 
- [TASTY (Python)](https://github.com/encryptogroup/tasty): combines garbled circuits with homomorphic encryption
- [ABY (C++)](https://github.com/encryptogroup/ABY): combines arithmetic, boolean and garbled style computation. Proposes protocols to switch between                                                       the arithmetic/boolean/garbled worlds for 2 parties
- [ABY3 (C++)](https://github.com/ladnir/aby3): extends ABY to 3 parties
- [ABY2.0](https://eprint.iacr.org/2020/1225.pdf): improves upon the ABY framework, provides a fast online phase with applications to PPML

## HE
- [TenSEAL (Python)](https://github.com/OpenMined/TenSEAL): A library for doing homomorphic encryption operations on tensors 
- [concrete (Rust)](https://github.com/zama-ai/concrete): zama.ai's variant of TFHE scheme. It is based on the Learning With Errors (LWE) and the Ring Learning With Errors (RLWE) problems

## SMPC
- [CrypTen (Python)](https://github.com/facebookresearch/CrypTen): a framework for Privacy Preserving Machine Learning built on PyTorch 
- [MP-SPDZ (C++)](https://github.com/data61/MP-SPDZ): software to benchmark various secure multi-party computation (MPC) protocols such as SPDZ, SPDZ2k, MASCOT, Overdrive, BMR garbled circuits, Yao's garbled circuits, and computation based on three-party replicated secret sharing as well as Shamir's secret sharing (with an honest majority) 
- [MOTION (C++)](https://github.com/encryptogroup/MOTION): a Framework for Mixed-Protocol Multi-Party Computation 


# Other Resources
- [awesome-ppml](https://github.com/mortendahl/awesome-ppml)
- [PPML - Resource](https://github.com/Ye-D/PPML-Resource)
- [awesome-homomorphic-encryption](https://github.com/jonaschn/awesome-he)
- [awesome-multi-party-computation](https://github.com/rdragos/awesome-mpc)
- [awesome-differential-privacy](https://github.com/menisadi/awesome-differential-privacy)
- [awesome-federated-learning](https://github.com/innovation-cat/Awesome-Federated-Machine-Learning#Videos-and-Lectures)
- [awesome-split-learning](https://github.com/splitlearning/awesome-split-learning)
