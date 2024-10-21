# Advancing Trust in AI Healthcare Machine Learning (HML) Models

This repository contains the code, Datasheet for MIMIC IV CRD, model card and fairness reports of the paper "Advancing Trust in Real-World Healthcare AI: A Framework for Enhanced Transparency and Fairness"

Healthcare Machine Learning (HML) models are revolutionizing the healthcare industry, promising improved patient outcomes and enhanced public health. However, the **black-box nature** of HML models raises concerns about **bias** and **trust**. To ensure these models are **reliable** and **trustworthy**, it is critical to examine the data they use and evaluate their **transparency**, **fairness**, and **accountability** alongside their predictive abilities.

## Study Overview

This study presents a **six-year systematic review** of risk prediction HML models using the **MIMIC clinical research database (CRD)**. The results were striking: for the popular **MIMIC IV – Intensive Care Unit (ICU) mortality task**, a naive baseline outperformed the state-of-the-art (SOTA) model, showing not only better predictive performance but also improved fairness among different patient groups, though some unfairness remains.

### Key Findings:
- **Naive baseline** outperformed the **SOTA model** in predictive performance for the ICU mortality task.
- Improved fairness across patient groups, though some unfairness was still observed.

These results highlight the **urgent need** for a robust framework to enhance the **trustworthiness** of HML models.

## Proposed Framework

We propose a three-step framework to ensure trustworthy HML models:

1. **Datasheet for CRD**:
   - Promotes **data transparency** and helps identify inherent **data bias**.
   - Inspired by recent recommendations for **datasheets in datasets**.

2. **Model Card**:
   - Provides detailed **model characteristics**, interpretable results, and evaluates performance across demographic groups.
   - Inspired by **model cards** for model reporting.

3. **Fairness Report**:
   - Thoroughly assesses and addresses any biases related to **sensitive attributes**, promoting **fairness** across all groups.

### Framework Benefits

This framework will assist practitioners by:
- **Identifying data anomalies** using the datasheet.
- Understanding **model structure** and its usage through the model card.
- Evaluating **fairness** results and their impact via the fairness report.

By following this framework, we aim to foster the development of **trustworthy** HML models that are **transparent**, **fair**, and **accountable**

# MIMIC IV v2.0 Datasheet

In the high-stakes context of healthcare, it is critical to ensure unbiased predictive outcomes. Despite the significant progress made in healthcare machine learning (HML), unfairness still exists due to the presence of biases in data and algorithms. Popular ML fairness strategies aim to assess and reduce algorithmic discrimination by imposing fairness constraints during model training. However, one of the inherent limitations of model-centric strategy is the data itself, which encodes real-world biases and inconsistencies, making it difficult to achieve fairness in healthcare settings. This highlights a need to reconsider fairness in the context of (i) the task and (ii) the data driving the model, and ways to make it a central part of any HML analysis.

To spark advances in fair HML and to aid practitioners, we present a comprehensive **Datasheet for MIMIC IV v2.0 CRD**, highlighting data inconsistencies across the database and includes task-specific feature-target analysis to streamline fairness evaluations for equitable decision-making in HML models. More than a mere inventory, the datasheet provides comprehensive insights into the database's 

## Contents
- [Motivation](MOTIVATION.md)
- [Composition](COMPOSITION.md)
- [Collection Process](COLLECTION_PROCESS.md)
- [Preprocessing/cleaning/labeling](PREPROCESSING_CLEANING.md)
- [Uses](USES.md)
- [Distribution](DISTRIBUTION.md)
- [Maintenance](MAINTENANCE.md)
- [Analysis - Risk Prediction Tasks](ANALYSIS_RISK_PREDICTION.md)

This datasheet, inspired by [Gebru et al., 2021](https://dl.acm.org/doi/pdf/10.1145/3458723) template, has been adapted for the intricacies of Clinical Research Databases (CRDs) and enriched to offer a thorough understanding of the data's fabric and its implications for HML tasks.


For more details, please refer to the complete MIMIC IV v2.0 datasheet provided in this repository.


# Model-Card 

For trustworthy HML modeling, model techniques and considerations play a crucial role in addition to the data. It is essential to know how a model was trained, the data it was exposed to, and its expected behavior in various scenarios. This information is vital for identifying potential biases and understanding the model's limitations. Our "Model card" provides detailed documentation of ML models, including their intended use, performance metrics, and evaluation results across different demographic groups. It facilitates informed decision-making by providing a comprehensive overview of a model's strengths and weaknesses, promoting transparency. It enables practitioners to assess whether a model is suitable for deployment in sensitive applications like healthcare, where the implications of biased or inaccurate predictions can be life-altering. We followed the ["Model Cards for Model Reporting"](https://arxiv.org/abs/1810.03993) framework to report on the analyzed HML models.

The provided model cards are based on the analysis and experiments conducted in the study "Advancing Trust in Real-World Healthcare AI: A Framework for Enhanced Transparency and Fairness" for ICU Mortality tasks,


## Contents
- [DuETT](DuETT.md)
- [STraTS](STraTS.md)
- [LSTM](LSTM.md)
- [XG Boost](XGBoost.md)
- [LR](LR.md)
