Notes

AI bias, also called machine learning bias or algorithm bias, refers to the occurrence of biased results due to human biases that skew the original training data or AI algorithm—leading to distorted outputs and potentially harmful outcomes.


Sources of bias

Distorted results can harm organizations and society at large. Here are a few of the more common types of AI bias7.

    Algorithm bias: Misinformation can result if the problem or question asked is not fully correct or specific, or if the feedback to the machine learning algorithm does not help guide the search for a solution.

    Cognitive bias: AI technology requires human input, and humans are fallible. Personal bias can seep in without practitioners even realizing it. This can impact either the dataset or model behavior.

    Confirmation bias: Closely related to cognitive bias, this happens when AI relies too much on pre-existing beliefs or trends in the data—doubling-down on existing biases, and unable to identify new patterns or trends.

    Measurement bias: Measurement bias is caused by incomplete data. This is most often an oversight or lack of preparation that results in the dataset not including the whole population that should be considered. For example, if a college wanted to predict the factors to successful graduation, but included only graduates, the answers would completely miss the factors that cause some to drop out.

    Out-group homogeneity bias: This is a case of not knowing what one doesn’t know. There is a tendency for people to have a better understanding of ingroup members—the group one belongs to—and to think they are more diverse than outgroup members. The result can be developers creating algorithms that are less capable of distinguishing between individuals who are not part of the majority group in the training data, leading to racial bias, misclassification and incorrect answers.

    Historical Bias: Training data may contain outdated views or discriminatory language, leading AI outputs to reflect historical biases.

    Representation Bias: Training data may underrepresent (or wholly omit) certain viewpoints, languages, or communities, skewing AI outputs toward the majority perspective.

    Prejudice bias: Occurs when stereotypes and faulty societal assumptions find their way into the algorithm’s dataset, which inevitably leads to biased results. For example, AI could return results showing that only males are doctors and all nurses are female.

    Recall bias: This develops during data labeling, where labels are inconsistently applied by subjective observations.

    Sample/Selection bias: This is a problem when the data used to train the machine learning model isn't large enough, not representative enough or is too incomplete to sufficiently train the system. If all school teachers consulted to train an AI model have the same academic qualifications, then any future teachers considered would need to have identical academic qualifications.

    Stereotyping bias: This happens when an AI system—usually inadvertently—reinforces harmful stereotypes. For example, a language translation system could associate some languages with certain genders or ethnic stereotypes. McKinsey gives a word of warning about trying to remove prejudice from datasets: “A naive approach is removing protected classes (such as sex or race) from data and deleting the labels that make the algorithm biased. Yet, this approach may not work because removed labels may affect the understanding of the model and your results’ accuracy may get worse.”


    How to Mitigate the Risk of AI Bias

    To manage the risk of AI bias in your outputs, you can adopt the following mitigation strategies. 

    1. Select the correct learning model:

    When using a supervised model, stakeholders select the training data. It’s critical that the stakeholder team be diverse—not just data scientists— and that they have had training to help prevent unconscious bias.
    Unsupervised models use AI alone to identify bias. Bias prevention tools need to be built into the neural network so that it learns to recognize what is biased.

    2. Train with the right data: Machine learning trained on the wrong data will produce wrong results. Whatever data is fed into the AI should be complete and balanced to replicate the actual demographics of the group being considered.

    3. Choose a balanced team: The more varied the AI team—racially, economically, by educational level, by gender and by job description—the more likely it will recognize bias. The talents and viewpoints on a well-rounded AI team should include AI business innovators, AI creators, AI implementers, and a representation of the consumers of this particular AI effort.9

    4. Perform data processing mindfully: Businesses need to be aware of bias at each step when processing data. The risk is not just in data selection: whether during pre-processing, in-processing or post-processing, bias can creep in at any point and be fed into the AI.

    5. Continually monitor: No model is ever complete or permanent. Ongoing monitoring and testing with real-world data from across an organization can help detect and correct bias before it causes harm. To further avoid bias, organizations should consider assessments by an independent team from within the organization or a trusted third-party.

    6. Avoid infrastructural issues: Aside from human and data influences, sometimes infrastructure itself can cause bias. For example, using data collected from mechanical sensors, the equipment itself could inject bias if the sensors are malfunctioning. This kind of bias can be difficult to detect and requires investment in the latest digital and technological infrastructures.

    Governance Strategies

        Understand the Data and the AI: Ensure your AI vendors are upholding AI governance principles of transparency, fairness, and explainability. Ask AI vendors about (and ensure they can clearly explain) the model’s data sources, training, safeguards, and bias-testing protocols.
        Create AI Output Benchmark: Regularly test the outputs to see if your AI model has regressed. You can set up a simple benchmark rubric in Excel, documenting the control input, the expected answer, the actual output, the rubric, and the resulting score. Especially for frequently automated or repeated tasks, regular benchmark tests will help you catch material regressions more quickly.
        Human Oversight: Perhaps most importantly, ensure human oversight, especially where AI is used in areas where bias is a significant concern (hiring decisions, lending decisions, law enforcement, etc.). Humans should be in the loop to meaningfully review AI outputs for bias, prejudice, or discrimination.



Reflections
AI’s power lies in its ability to quickly synthesize vast amounts of data and generate actionable insights, but its outputs can reflect biases that arise across the AI lifecycle. By taking an informed approach to AI use and implementing mitigation strategies, business and legal professionals can harness the benefits of AI while avoiding the costly pitfalls of AI bias.


https://pacific.ai/unmasking-the-biases-within-ai-how-gender-ethnicity-religion-and-economics/

https://www.crescendo.ai/blog/ai-bias-examples-mitigation-guide



https://www.ibm.com/think/topics/ai-bias
https://www.summitlaw.com/law-blog/ai-bias-and-how-to-mitigate-it



