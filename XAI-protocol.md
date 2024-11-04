## XAI Protocol

The integration of XAI across the machine learning classification model development lifecycle often lacks systematic implementation, particularly during the model improvement phase, leading to inconsistent and potentially suboptimal utilisation of explanatory insights. To address this gap, we propose a comprehensive protocol for selecting, implementing, and evaluating XAI approaches throughout the model development lifecycle. This protocol comprises seven interconnected stages: initial XAI approach selection based on context-of-use, model characteristics and stakeholder requirements; systematic model diagnosis using selected XAI methods; comparative testing of multiple XAI approaches for shortlisting; integration of XAI insights for model improvement; quantitative evaluation of XAI effectiveness (alongside evaluating classifiers and visualisation strategies); structured stakeholder communication; and continuous monitoring and refinement. The protocol addresses the current ad hoc nature of XAI implementation by providing a structured framework that ensures consistent application of explainability methods, facilitates quantifiable improvement in both model performance and explanation quality, and enables effective stakeholder engagement throughout the development process. 

1. Initial XAI Approach Selection:

- Define context-of-use and explanation requirements (local vs. global, feature attribution needs)
  
- Evaluate model characteristics (complexity, architecture, input data type)

- Match XAI methods to stakeholder expertise and needs

- Create a shortlist of potentially suitable XAI approaches

2. Model Diagnosis:

- Apply selected XAI methods to analyze:

  * Feature importance patterns across different data segments

  * Decision boundary characteristics

  * Model behavior on edge cases and outliers

  * Potential biases or systematic errors

- Document all findings systematically

- Create baseline measurements for model behavior

3. Testing and Comparison:
   
- Implement multiple shortlisted XAI approaches

- Compare explanations for:

  * Consistency across different instances

  * Stability across similar inputs

  * Agreement between different methods

- Further refine/shortlist XAI approaches
  
- Document discrepancies and insights gained from each method
  
4. Model Improvement Integration:

- Use XAI insights to:

  * Refine feature engineering approaches

  * Adjust model architecture or parameters

  * Address identified biases or performance gaps

  * Enhance robustness in problematic areas

- Measure impact of each improvement

- Document relationship between XAI insights and improvements made

4. Model Selection: (Including classifier, XAI approach & visualisations)

- Define quantitative metrics for XAI performance:

  * Explanation consistency

  * Computational efficiency

  * Stakeholder comprehension

  * Alignment with domain knowledge

- Conduct comparative analysis across different XAI methods using quantitative metrics

- Conduct comparative evaluation of different classification models using established processes (e.g. following recommendations of TRIPOD+AI)

- Conduct comparative evaluation of different visualisation strategies for summarising/communicating classifier predictive performance and explanations from selected XAI methods
  
- Document discrepancies and insights gained from each method/combinations of methods

- Evaluate trade-offs between explainability and model performance

- Select optimal XAI approach based on quantitative results

5. Stakeholder Communication:

- Create layered communication strategy:
  
  * Executive summaries for high-level stakeholders

  * Detailed technical documentation for developers

  * User-friendly explanations for end-users

- Implement feedback mechanisms

- Maintain traceability between decisions and explanations

- Provide interactive exploration tools where appropriate

6. Continuous Monitoring and Refinement:

- Track explanation quality over time, monitoring performance drifts

- Monitor stakeholder feedback and understanding

- Adjust explanations based on evolving needs

- Document all changes and their rationale

# This systematic approach ensures:

- Consistent application of XAI throughout the lifecycle

- Clear documentation of decision-making processes

- Quantifiable improvement in model and explanation quality

- Effective stakeholder engagement and understanding

This systematic approach enables relevant stakeholders (from developers to end-users) to make informed decisions about XAI method selection, implementation, and interpretation, while maintaining traceability between model improvements and explanatory insights.

Practical implementation of the proposed protocol and demonstration of XAI integration across the full classification model development lifecycle is explored through several case studies which tackle diverse data types, types of classification problems, and types of classification models:

* [Case study 1: Image classification](./case-study-image.md)

* [Case study 2: Video classification](./case-study-video.md)

* [Case study 3: Structured data classification](./case-study-stdata.md) 

