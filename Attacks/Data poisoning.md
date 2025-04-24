# Data poisoning 
Data poisoning is a type of attack on machine learning (ML) and artificial intelligence (AI) models where an adversary intentionally manipulates the training data to compromise the model's performance. Here’s a brief overview:

## What is Data Poisoning?
- Data poisoning involves injecting malicious data into the training dataset of an AI model. This can lead to the model learning incorrect patterns, making it unreliable or biased. The goal of the attacker can vary, including:
- Degrading Model Performance: Making the model less accurate or effective.
- Biasing the Model: Introducing biases that cause the model to make specific, incorrect predictions.
- Backdoor Attacks: Embedding hidden triggers in the model that cause it to behave maliciously when specific inputs are encountered.

## How Does It Work?
- Insertion of Malicious Data: Attackers add carefully crafted data points to the training set.
- Model Training: The model is trained on this poisoned dataset, learning from both legitimate and malicious data.
- Deployment: Once deployed, the model may perform poorly or exhibit unexpected behaviors due to the influence of the poisoned data.

## Examples and Impacts
- Spam Filters: Poisoning a spam filter could make it classify spam emails as legitimate.
- Facial Recognition: Introducing biased data could make a facial recognition system less accurate for certain demographics.
- Autonomous Vehicles: Poisoned data could lead to incorrect object detection, posing safety risks.

## Mitigation Strategies
- Data Validation: Implementing rigorous checks to ensure data integrity.
- Robust Training Methods: Using techniques that make models less sensitive to outliers and anomalies.
- Continuous Monitoring: Regularly evaluating model performance to detect unusual patterns. Including https://learn.microsoft.com/en-us/azure/defender-for-cloud/ai-threat-protection and https://learn.microsoft.com/en-us/purview/

Additional resources:
- https://www.ibm.com/think/topics/data-poisoning
- https://www.techradar.com/news/what-is-data-poisoning-and-how-do-we-stop-it
- https://www.techtarget.com/searchEnterpriseAI/definition/data-poisoning-AI-poisoning
