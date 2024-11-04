## XAI Focus Group Results

## Research domains

The main research domains of the participants in the XAI focus groups were: 

1) Computer vision/Medical image computing (53.8%)

2) Healthcare/Medical records (23.1%)

3) Natural language processing (7.7%)

4) Applied mathematics/statistics (7.7%)

5) Bioinformatics/microscopy (7.7%)

<img src="research-domains-pie-svg-adjusted.svg" width="50%">

## Data types

The different types of data used by the participants in their research were:

1) Images (43.75%)

2) Time-series data (25%)

3) Structured data (18.75%)

4) Multi-modal data (12.5%)

<img src="data-types-pie-svg.svg" width="50%">


## Types of classification tasks

The types of classification tasks tackled by different participants in their research were grouped in five categories. These are described below along with a summary of participant responses.

1) Binary classification (36.4%)

2) Small multi-class (3 - 10 classes) classification (50%)

3) Large multi-class (>10 classes) classification (0%)

4) Small multi-label (3 - 10 classes) classification (9.1%)

5) Large multi-label (>10 classes) classification (4.5%)

Small multi-class classification is the most common type of classification problem encountered while no participants reported working on large multi-class classification tasks.

<img src="classification-types-pie-svg.svg" width="50%">


## How is XAI used throughout the model development lifecycle?

Apart from understanding the research domains, types of data and classification tasks and types of XAI approaches prevalent in literature and adopted by focus group participants, this survey is designed to evaluate the usage of XAI across four stages of the ML development lifecycle (for classification tasks):

1) Model Diagnosis - assessing how XAI is used to understand model behavior and error patterns

2) Model Improvement - evaluating how XAI insights are used to enhance model performance

3) Model Selection - understanding how XAI influences the choice of methods and visualisation techniques and whether the rigour applied to selecting the best performing classifiers for a given task are extended to selection of XAI and visualisation approaches

4) Stakeholder Communication - examining how XAI is used to explain models and decisions to various stakeholders

Analysis of the focus group responses reveals distinct patterns in how XAI methods are currently employed within the machine learning development lifecycle. The predominant application centers on model diagnosis, with a particular emphasis on feature importance interpretation and sanity checking procedures. Notably, 10 out of 13 participants reported using XAI for these fundamental diagnostic purposes, indicating a strong consensus around its utility in understanding model behavior at a basic level.

The visualisation approaches employed by practitioners demonstrate a reliance on conventional performance metrics, with ROC curves and confusion matrices being ubiquitously cited. While some participants reported using more sophisticated techniques such as occlusion maps and latent space visualisation, there appears to be a significant gap between the theoretical potential of XAI visualisation methods discussed in current literature and their practical implementation. This disparity is particularly evident in the limited adoption of interactive and dynamic visualisation techniques that could enhance stakeholder engagement and understanding.

When examining model improvement applications, the responses indicate less consistent utilisation of XAI methods compared to diagnostic purposes. While practitioners acknowledge the potential for XAI to inform feature selection and evaluate model robustness, there appears to be limited systematic integration of XAI insights into the iterative improvement process. This contrasts markedly with current literature, which emphasises the potential for XAI to drive targeted model refinements and architectural decisions throughout the development cycle, but is consistent with practical usage evident in recent literature.

Stakeholder communication emerged as a particularly challenging aspect of XAI implementation. Several participants noted the difficulty in conveying complex explanations to diverse audiences, with one participant specifically highlighting the varying receptiveness of medical professionals to different visualisation approaches. This finding aligns with current literature emphasizing the need for audience-specific explanation strategies, but suggests that practical implementation of such targeted approaches remains challenging.

Current literature in XAI emphasises the importance of systematic evaluation frameworks and quantitative metrics for assessing explanation quality. However, the focus group responses indicate limited adoption of such formal evaluation approaches, with practitioners instead relying primarily on qualitative assessment and stakeholder feedback. Again, while XAI focused literature highlight the importance of quantitative evaluation of explanations, this is seldom explored in wider literature when the focus is on developing/evaluating classification models for specific applications. This represents a significant opportunity for improvement in XAI implementation practices.

To address these gaps, several evidence-based recommendations emerge from current literature. First, ML practitioners should consider implementing structured protocols for XAI method selection and evaluation, incorporating quantitative metrics such as faithfulness measures and stability assessments. Second, the development of stakeholder-specific visualisation strategies should be prioritized, with particular attention to the varying technical literacy levels of different audiences. Third, practitioners should expand their use of XAI beyond post-hoc explanation to include early-stage model development decisions, including leveraging XAI to inform model improvements and incorporating quantitative approaches for XAI-informed classification model selection.

According to current literature, the model improvement stage is where XAI usage is least prevalent in the development lifecycle. This is paradoxiacal as XAI approaches could provide valuable insights for improving model performance. Majority of recent literature tackling classification problems (particularly those based on deep neural networks, __references to be added__) use XAI for model diagnosis, model selection and stakeholder communication, albeit, its use in the last stage tends to be ad-hoc and largely qualitative. Furthermore, current research literature indicates significant gaps in standardising the process for how XAI is selected and used throughout the development lifecycle and processes for documenting the same in a manner that maintains consistency across different stakeholder groups while preserving technical rigor. These factors emphasise the need for a structured protocol that assists ML practictioners in selecting and using XAI approaches throughout the model development lifecycle for specific classification problems of interest, which is notably absent in current literature despite its critical importance. While numerous XAI techniques have been developed and deployed, their application remains largely ad-hoc, with different studies adopting varying approaches at different stages of model development. This lack of standardisation leads to several challenges: inconsistent explanation quality within and across applications, difficulty in comparing XAI effectiveness between different models, and potential gaps in model understanding when transitioning between development stages. The absence of a systematic protocol is particularly problematic in the model improvement stage, where XAI insights could significantly enhance model refinement but are often underutilised. Current literature focuses predominantly on developing new XAI techniques or applying existing ones for specific use cases, rather than establishing a comprehensive framework for when and how to apply XAI methods throughout the entire model lifecycle. A standardized protocol would not only ensure consistent and comprehensive use of XAI across all development stages but would also provide clear guidelines for selecting appropriate XAI techniques based on the context-of-use, model type, stakeholder needs, and specific development stage requirements.

The integration of automated XAI pipelines represents a promising direction for improving current practices. Such pipelines could standardise the evaluation of explanation quality and facilitate continuous monitoring of model behavior, addressing the current ad-hoc approach evident in focus group responses and recent literature in the domain. Furthermore, the development of interactive explanation interfaces could bridge the gap between technical capability and stakeholder comprehension, addressing the communication challenges highlighted by multiple participants.

Given this gap in current literature and the need for a standardised protocol for adopting XAI in classification model development, we propose an XAI protocol based on insights dervied from the conducted focus groups, survey of relevant literature and empirical investigations.

[XAI Protocol](./XAI-protocol.md)

