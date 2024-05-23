COMET is an initiative from the [NetSys lab](https://netsys.doc.ic.ac.uk/) at Imperial College London. COMET aims to answer the question: Can we use novel confidential computing architectures to provide private, trusted, personalised, and dynamically-configurable machine-learning models on consumer devices to cater for heterogenous environments and user requirements?  

This website provides an overview of the projects within COMET. 

## GuaranTEE: Towards Attestable and private ML with CCA

**Abstract**: Machine-learning (ML) models are increasingly being deployed on edge devices to provide a variety of services. However, their deployment is accompanied by challenges in model privacy and auditability. Model providers want to ensure that (i) their proprietary models are not exposed to third parties; and (ii) be able to get attestations that their genuine models are operating on edge devices in accordance with the service agreement with the user. Existing measures to address these challenges have been hindered by issues such as high overheads and limited capability (processing/secure memory) on edge devices. In this work, we propose GuaranTEE, a framework to provide attestable private machine learning on the edge. GuaranTEE uses Confidential Computing Architecture (CCA), Arm’s latest architectural extension that allows for the creation and deployment of dynamic Trusted Execution Environments (TEEs) within which models can be executed. We evaluate CCA’s feasibility to deploy ML models by developing, evaluating, and openly releasing a prototype. We also suggest improvements to CCA to facilitate its use in protecting the entire ML deployment pipeline on edge devices.

Paper can be found [here](https://arxiv.org/pdf/2404.00190).

Code can be found [here](https://github.com/comet-cc/GuaranTEE).

A short video on GuaranTEE can be found [here](https://youtu.be/Jx_cGV-KTns).

### Citation
```
@inproceedings{Siby24GuaranTEE,
  title     = {GuaranTEE: Towards Attestable and private ML with CCA},
  author    = {Sandra Siby, Sina Abdollahi, Mohammad Maheri, Marios Kogias, Hamed Haddadi},
  booktitle = {The 4th Workshop on Machine Learning and Systems (EuroMLSys)},
  year      = {2024}
}
```

## Contact

In case of questions regarding the code, please get in touch with [Sina Abdollahi](https://www.imperial.ac.uk/people/s.abdollahi22) and [Sandra Siby](https://sandrasiby.github.io/). 