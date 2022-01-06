# Privacy-preserving Machine Learning: Resources and Materials

## Table of Contents
1. [About](#about)
2. [Secure Machine Learning](#secure-machine-learning)
4. [Courses](#courses)
5. [Other Resources](#other-resources)

## About
This is a compiled list of resources and materials for PPML.  

## Secure Machine Learning  
### Training Phase
#### Homomorphic Encryption (HE) & Functional Encryption (FE)

1. [BMC medical genomics’18] [Privacy-preserving logistic regression training](https://bmcmedgenomics.biomedcentral.com/articles/10.1186/s12920-018-0398-y)
2. [Arxiv’19] [CryptoNN: Training Neural Networks over Encrypted Data](https://arxiv.org/abs/1904.07303) (FE)
3. [PETS’18] [CryptoDL: Privacy-preserving Machine Learning as a Service](https://petsymposium.org/2018/files/papers/issue3/popets-2018-0024.pdf)
4. [*IEEE/CVF’19*] [Towards Deep Neural Network Training on Encrypted Data](https://ieeexplore.ieee.org/document/9025601)
5. [ArXiv’20] [Neural Network Training With Homomorphic Encryption](https://arxiv.org/abs/2012.13552)
6. [ArXiv’20] [PrivFT: Private and Fast Text Classification with Homomorphic
Encryption](https://arxiv.org/abs/1908.06972?utm_source=feedburner&utm_medium=feed&utm_campaign=Feed%253A+arxiv%252FQSXk+%2528ExcitingAds%2521+cs+updates+on+arXiv.org%2529)
7. [NDSS’21] [POSEIDON: Privacy-Preserving Federated Neural Network Learning](https://arxiv.org/abs/2009.00349).

#### Secure Multi-Party Computation (SMPC)

1. [S&P’17] [SecureML: A System for Scalable Privacy-Preserving Machine Learning](https://eprint.iacr.org/2017/396)
2. [CCS’19] [QUOTIENT: two-party secure neural network training and prediction](https://dl.acm.org/citation.cfm?id=3339819)
3. [Arxiv’19] [CodedPrivateML: A Fast and Privacy-Preserving Framework for Distributed Machine Learning](https://arxiv.org/abs/1902.00641)
4. [PETS’20] [FALCON: Honest-Majority Maliciously Secure Framework for Private Deep Learning](https://arxiv.org/abs/2004.02229). [Code](https://github.com/snwagh/falcon-public) (C++).
5. [ICPP’20] [ParSecureML: An Efficient Parallel Secure Machine Learning Framework on GPUs](https://dl.acm.org/doi/pdf/10.1145/3404397.3404399). [Code](https://github.com/ZhengChenCS/ParSecureML) (C++).
6. [PoPETs’20] [FLASH: Fast and Robust Framework for Privacy-preserving Machine Learning](https://eprint.iacr.org/2019/1365)
7. [NDSS’20] [BLAZE: Blazing Fast Privacy-Preserving Machine Learning](https://eprint.iacr.org/2020/042)
8. [USENIX’21] [Cerebro: A Platform for Multi-Party Cryptographic Collaborative Learning](https://www.usenix.org/conference/usenixsecurity21/presentation/zheng). [Code](https://github.com/mc2-project/cerebro) (Python).
9. [USENIX’21] [Fantastic Four: Honest-Majority Four-Party Secure Computation With Malicious Security](https://www.usenix.org/system/files/sec21fall-dalskov.pdf)
10. [S&P’21] [CryptGPU: Fast Privacy-Preserving Machine Learning on the GPU](http://arxiv.org/abs/2104.10949). [Code](https://github.com/jeffreysijuntan/CryptGPU) (Python).
11. [USENIX 2021] [SWIFT: Super-fast and Robust Privacy-Preserving Machine Learning](https://www.semanticscholar.org/paper/SWIFT%3A-Super-fast-and-Robust-Privacy-Preserving-Koti-Pancholi/55e9017bcf4ffec2d34c760cc832d72e39c73216)
12. [Arxiv’21] [Adam in Private: Secure and Fast Training of Deep Neural Networks with Adaptive Moment Estimation](https://arxiv.org/abs/2106.02203).
13. [Arxiv’21] [Tetrad: Actively Secure 4PC for Secure Training and Inference](https://arxiv.org/abs/2106.02850)
14. [Arxiv’21] [Secure Quantized Training for Deep Learning](https://arxiv.org/abs/2107.00501)

#### Hybrid Techniques

1. [IACR Cryptol’17] [Private Collaborative Neural Network Learning](https://eprint.iacr.org/2017/762.pdf) (SMPC + DP)
2. [CCS’18] [ABY3: A Mixed Protocol Framework for Machine Learning](https://eprint.iacr.org/2018/403.pdf). [Code](https://github.com/ladnir/aby3) (C++).
3. [PETS’18] [SecureNN: 3-Party Secure Computation for Neural Network Training](https://eprint.iacr.org/2018/442.pdf). [Code](https://github.com/snwagh/securenn-public) (C++).
4. [NeurlPS’20] [Glyph: Fast and Accurately Training Deep Neural Networks on Encrypted Data](https://arxiv.org/pdf/1911.07101.pdf)
5. [NDSS’20] [Trident: Efficient 4PC Framework for Privacy Preserving Machine Learning](https://eprint.iacr.org/2019/1315)

### Inference Phase

#### Homomorphic Encryption (HE) & Functional Encryption (FE)

1. [ICML’16] [CryptoNets: Applying Neural Networks to Encrypted Data with High Throughput and Accuracy](https://proceedings.mlr.press/v48/gilad-bachrach16.html). [Code](https://github.com/microsoft/CryptoNets) (C#).

### Secure Multi-Party Computation (SMPC)

1. [SIGSAC’17] [Oblivious Neural Network Predictions via MiniONN Transformations](https://eprint.iacr.org/2017/452.pdf)
2. [ASIACCS’18] [Chameleon: A Hybrid Secure Computation Framework for Machine Learning Applications](https://arxiv.org/abs/1801.03239)

## Courses
- [Private AI Series (OpenMined)](https://courses.openmined.org/courses).
- [MIT 6.875: Foundations of Cryptography](https://mit6875.github.io/)  (Fall 2021)  - [Lecture Notes](https://khoaduynguyen.com/tags/mit6-875/).  
- [Privacy in Statistics and Machine Learning](https://dpcourse.github.io/schedule.html) (Spring 2021).    
- [Algorithms for Private Data Analysis - Fall 2020](http://www.gautamkamath.com/CS860-fa2020.html) (Fall 2020).    
- [Privacy Preserving Machine Learning](http://researchers.lille.inria.fr/abellet/teaching/private_machine_learning_course.html).    

## Other Resources
- [awesome-ppml](https://github.com/mortendahl/awesome-ppml)
- [PPML - Resource](https://github.com/Ye-D/PPML-Resource)
- [awesome-homomorphic-encryption](https://github.com/jonaschn/awesome-he)
- [awesome-multi-party-computation](https://github.com/rdragos/awesome-mpc)
- [awesome-differential-privacy](https://github.com/menisadi/awesome-differential-privacy)
- [awesome-federated-learning](https://github.com/innovation-cat/Awesome-Federated-Machine-Learning#Videos-and-Lectures)
- [awesome-split-learning](https://github.com/splitlearning/awesome-split-learning)
