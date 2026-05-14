COMET is an initiative from the [NetSys lab](https://netsys.doc.ic.ac.uk/) at Imperial College London. COMET aims to answer the question: Can we use novel confidential computing architectures to provide private, trusted, personalised, and dynamically-configurable machine-learning models on consumer devices to cater for heterogenous environments and user requirements?  

This website provides an overview of the projects within COMET. 

## Other

## AgenTEE: Confidential LLM Agent Execution on Edge Devices

**Abstract**: Large Language Model agents enable powerful automation but create expansive attack surfaces through integration with non-deterministic models and third-party services. While cloud deployments dominate currently, edge execution is increasingly common to reduce latency and enhance privacy. However, securing complex agent pipelines on edge devices remains challenging when protecting proprietary assets and sensitive runtime state across heterogeneous, potentially compromised platforms.

We present AgenTEE, a system that deploys confidential agent pipelines on edge devices. AgenTEE places the agent runtime, inference engine, and third-party applications into independently attested confidential virtual machines (cVMs) and mediates all interaction through explicit, verifiable communication channels. Built on Arm Confidential Compute Architecture (CCA), AgenTEE enforces strong system-level isolation of sensitive assets and runtime state. Our evaluation demonstrates practical feasibility, achieving near-native performance with less than 5.15% overhead compared to commodity OS multi-process deployments.

Paper can be found [here](https://arxiv.org/pdf/2604.18231).

Code can be found [here](https://github.com/comet-cc/AgenTEE).

## CAEC: Confidential, Attestable, and Efficient Inter-CVM Communication with Arm CCA

**Abstract**: Confidential Virtual Machines (CVMs) are increasingly adopted to protect sensitive workloads from privileged adversaries such as the hypervisor. While they provide strong isolation guarantees, existing CVM architectures lack first-class mechanisms for inter-CVM data sharing due to their disjoint memory model, making inter-CVM data exchange a performance bottleneck in compartmentalized or collaborative multi-CVM systems. Under this model, a CVM’s accessible memory is either shared with the hypervisor or protected from both the hypervisor and all other CVMs. This design simplifies reasoning about memory ownership; however, it fundamentally precludes plaintext data sharing between CVMs because all inter-CVM communication must pass through hypervisor-accessible memory, requiring costly encryption and decryption to preserve confidentiality and integrity.

In this paper, we introduce CAEC, a system that enables protected memory sharing between CVMs. CAEC builds on Arm Confidential Compute Architecture (CCA) and extends its firmware to support Confidential Shared Memory (CSM), a memory region securely shared between multiple CVMs while remaining inaccessible to the hypervisor and all non-participating CVMs. CAEC’s design is fully compatible with CCA hardware and introduces only a modest increase (4%) in CCA firmware code size. CAEC delivers substantial performance benefits across a range of workloads. For instance, inter-CVM communication over CAEC achieves up to 209x reduction in CPU cycles compared to encryption-based mechanisms over hypervisor-accessible shared memory. By combining high performance, strong isolation guarantees, and attestable sharing semantics, CAEC provides a practical and scalable foundation for the next generation of trusted multi-CVM services across both edge and cloud environments.

Paper can be found [here](https://arxiv.org/pdf/2512.01594).

Code can be found [here](https://github.com/comet-cc/CAEC).

## GuaranTEE: Towards Attestable and private ML with CCA

**Abstract**: Machine-learning (ML) models are increasingly being deployed on edge devices to provide a variety of services. However, their deployment is accompanied by challenges in model privacy and auditability. Model providers want to ensure that (i) their proprietary models are not exposed to third parties; and (ii) be able to get attestations that their genuine models are operating on edge devices in accordance with the service agreement with the user. Existing measures to address these challenges have been hindered by issues such as high overheads and limited capability (processing/secure memory) on edge devices. In this work, we propose GuaranTEE, a framework to provide attestable private machine learning on the edge. GuaranTEE uses Confidential Computing Architecture (CCA), Arm’s latest architectural extension that allows for the creation and deployment of dynamic Trusted Execution Environments (TEEs) within which models can be executed. We evaluate CCA’s feasibility to deploy ML models by developing, evaluating, and openly releasing a prototype. We also suggest improvements to CCA to facilitate its use in protecting the entire ML deployment pipeline on edge devices.

Paper can be found [here](https://arxiv.org/pdf/2404.00190).

Code can be found [here](https://github.com/comet-cc/GuaranTEE).

## Contact

In case of questions regarding the code, please get in touch with [Sina Abdollahi](https://www.imperial.ac.uk/people/s.abdollahi22) and [Sandra Siby](https://sandrasiby.github.io/). 
