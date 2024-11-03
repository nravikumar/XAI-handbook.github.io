## XAI Protocol

<div align="justify">
This repository summarises findings from a series of focus groups conducted to understand how explainable AI (XAI) is used in current practice when building classification models. Insights from the focus groups, survey of relevant literature and empirical investigations are used to establish a set of recommendations for implementing XAI techniques in classification models. The core mission is to provide a set of best practices, i.e. establish an XAI protocol, that enables relevant stakeholders to make effective use of XAI in their model development lifecycle. 
</div>

## XAI in the model development lifecycle

<div align="justify">
The role of XAI evolves throughout different stages of developing a classification model, each serving a unique purpose. The different stages of the model development lifecycle may be broadly categorised as: model diagnosis, model improvement, model selection and communicating model outputs to relevant stakeholders. During model diagnosis, XAI is used to understand how a model works. This typically includes identifying biases or spurious correlations in the data which impact model predictions, understanding the types of prediction errors and reasons for the same, and identifying which features are relevant/important for the classification task at hand. 
</div>

<div align="justify">
In the model improvement stage, XAI methods are used to enhance the model's predictive performance in various ways. For instance they can - quantitatively evaluate how well the model handles outliers and biases in the data, allowing for model refinement, and appropriate mitigation strategies to be implemented; compare how different classifiers prioritise features, enabling consensus-based identification of important features, which in turn may be used to refine the model(s) of interest; analyse how well specific features distinguish between different classes, encouraging class-specific enhancement of the strategy employed for training the classifier; and pinpoint which cases are straightforward to classify versus those that prove more challenging, for each model investigated, allowing for refinement of the model(s) to tackle challenging cases or encouraging adoption of appropriate ensembling approaches. All these insights help create a more robust and reliable classification model. 
</div>

<div align="justify">
When it comes to model selection, there's often a critical blind spot in current practices. While most studies compare accuracy, precision, recall, and other standard classification metrics to choose the best model, they rarely apply the same rigorous evaluation to selecting the most appropriate XAI techniques or visualization methods. This oversight means that while high-performing classifiers are often produced and reported, they are seldom accompanied by effective tools for explaining or visualising their decisions. As a result they often don't effectively communicate their reasoning to end users, which is crucial for real-world applications. 
</div>

<div align="justify">
Finally, XAI plays a multifaceted role in the stakeholder communication stage serving as a bridge between technical implementation and practical use. This includes, translating complex model mechanisms into accessible and understandable information, understanding the implications of model decisions and the context-of-use within which the model's use is safe/appropriate, providing actionable insights that support subsequent informed decision-making by the stakeholders, and generating evidence-based justifications for model design choices, to name a few. This stage of the model development lifecycle must therefore include comprehensive documentation comprising - the diagnostic methodology, improvement strategies, and model selection criteria adopted, establishing clear traceability between identified issues and implemented solutions throughout the development lifecycle; local (sample-specific) and global (across groups or sub-groups, e.g. dataset, class, attributes) explanations to contextualise model performance within the specific domain of application; and accessible justifications for overall conclusions and end-user facing decisions, employing appropriate levels of technical detail for different stakeholder groups while maintaining scientific rigor.
</div>
