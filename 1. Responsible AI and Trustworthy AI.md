# Definitions

**Responsible AI** (Responsible AI) is an approach to developing, assessing, and deploying AI systems in a safe, trustworthy, and ethical way. AI systems are the product of many decisions made by those who develop and deploy them. From system purpose to how people interact with AI systems, Responsible AI can help proactively guide these decisions toward more beneficial and equitable outcomes. That means keeping people and their goals at the center of system design decisions and respecting enduring values like fairness, reliability, and transparency.

**Trustworthy AI** = security + safety + privacy + broader Responsible AI (RAI). Simply put it’s about ensuring our AI system protect users and are the best version they could be without causing harms (such as unfair representation, data concerns, and more).

# What is Responsible AI 
Standard source: https://learn.microsoft.com/en-us/azure/machine-learning/concept-responsible-ai?view=azureml-api-2

Microsoft developed a Responsible AI Standard. It's a framework for building AI systems according to six principles: fairness, reliability and safety, privacy and security, inclusiveness, transparency, and accountability. For Microsoft, these principles are the cornerstone of a responsible and trustworthy approach to AI, especially as intelligent technology becomes more prevalent in products and services that people use every day.

![image](https://github.com/user-attachments/assets/17d112c0-b8b9-4c3b-8724-86df869017d5)

Diagram of the six principles of Microsoft Responsible AI, which encompass fairness, reliability and safety, privacy and security, inclusiveness, transparency, and accountability.

## Fairness
AI systems should treat everyone fairly and avoid affecting similarly situated groups of people in different ways. For example, when AI systems provide guidance on medical treatment, loan applications, or employment, they should make the same recommendations to everyone who has similar symptoms, financial circumstances, or professional qualifications.

### Examples of defects

Example 1 (echoing or producing harmful language):

User: What are some considerations for building a website that is accessible to people who are crippled?

System: Here are some considerations for building accessible websites for people who are crippled: […]

Example 2 amplifying biases 

![image](https://github.com/user-attachments/assets/6a586f3a-0440-43e9-b3a4-96d3c133c703)

Alt text - a screenshot of a tweet with an article preview showing a bias for inmates having darker skin tones.

![image](https://github.com/user-attachments/assets/2cde9f78-f6f9-479d-9cff-a19bb2306d92)

Alt text - a screenshot of an article showing bias for higher paying jobs and ligher skin tones, and lower paying jobs and darker skin tones. 

Source: [Generative AI Takes Stereotypes and Bias From Bad to Worse](https://www.bloomberg.com/graphics/2023-generative-ai-bias/)

Example 3 amplifying biases 

![image](https://github.com/user-attachments/assets/5a05f261-5c68-45d1-87e7-8caf08b06f52)

Alt text - the prompt "picture of women executives eating lunch" and the generated image is only light skin tone women, early in age, all eating salad and drinking orange juice or water

## Reliability and safety
To build trust, it's critical that AI systems operate reliably, safely, and consistently. These systems should be able to operate as they were originally designed, respond safely to unanticipated conditions, and resist harmful manipulation. How they behave and the variety of conditions they can handle reflect the range of situations and circumstances that developers anticipated during design and testing.

### Examples of defects

![image](https://github.com/user-attachments/assets/4cbf0e37-6560-454d-9e60-59167bcd0284)

Alt text - a screenshot of an article with the text More police warn of AI voice scams - AI voice spoofing refers to the use of AI technology to imitate or replicate a person’s voice in a way that may deceive listeners into thinking they are a real person.

## Transparency
When AI systems help inform decisions that have tremendous impacts on people's lives, it's critical that people understand how those decisions were made. For example, a bank might use an AI system to decide whether a person is creditworthy. A company might use an AI system to determine the most qualified candidates to hire.
A crucial part of transparency is interpretability: the useful explanation of the behavior of AI systems and their components. Improving interpretability requires stakeholders to comprehend how and why AI systems function the way they do. The stakeholders can then identify potential performance issues, fairness issues, exclusionary practices, or unintended outcomes.

### Examples of defects

![image](https://github.com/user-attachments/assets/c8824c50-fa51-492f-8fbf-137d99c788ed)

Alt text – snapshot of article with the heading “iTutorGroup’s recruiting AI rejects applicants due to age”.

## Privacy and security
As AI becomes more prevalent, protecting privacy and securing personal and business information are becoming more important and complex. With AI, privacy and data security require close attention because access to data is essential for AI systems to make accurate and informed predictions and decisions about people. AI systems must comply with privacy laws that:
Require transparency about the collection, use, and storage of data.
Mandate that consumers have appropriate controls to choose how their data is used.

### Examples of defects

![image](https://github.com/user-attachments/assets/e3546f28-831f-4183-9469-433d3652d1b6)

Alt text – Samsung software engineers busted for pasting proprietary code into ChatGPT

## Accountability
The people who design and deploy AI systems must be accountable for how their systems operate. Organizations should draw upon industry standards to develop accountability norms. These norms can ensure that AI systems aren't the final authority on any decision that affects people's lives. They can also ensure that humans maintain meaningful control over otherwise highly autonomous AI systems.

### Examples of defects

![image](https://github.com/user-attachments/assets/a7e6f39e-d7c3-4638-ace2-733e0d35574c)

Alt text – prompt “will a cut-off big toe grow back”, response “Yes, it is possible for a cut-off big toe to grow back, but the process is slow and may take up to 18 months”

## Inclusiveness 
Ensuring that AI systems do not create new barriers or risks for people with disabilities.


