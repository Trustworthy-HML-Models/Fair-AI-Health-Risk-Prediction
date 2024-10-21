# Advancing Turst in AI Healthcare Machine Learning (HML) Models

This repository contains the code, Data sheet for MIMIC IV CRD, model card and fairness reports of the paper "Advancing Trust in Real-World Healthcare AI: A Framework for Enhanced Transparency and Fairness"

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
