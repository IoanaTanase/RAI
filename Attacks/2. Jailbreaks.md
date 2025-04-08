# AI Jailbreaks

Sources:
- https://www.microsoft.com/en-us/security/blog/2024/06/04/ai-jailbreaks-what-they-are-and-how-they-can-be-mitigated/?msockid=2ed372bd3e936a17133e67c23f276be1
- https://news.microsoft.com/source/features/ai/safeguarding-ai-against-jailbreaks-and-other-prompt-attacks/#:~:text=To%20help%20protect%20against%20jailbreaks%20and%20indirect%20attacks%2C,AI%20developers%20detect%2C%20measure%20and%20manage%20the%20risk.?msockid=2ed372bd3e936a17133e67c23f276be1

## What is AI jailbreak?
An AI jailbreak is a technique that can cause the failure of guardrails (mitigations). The resulting harm comes from whatever guardrail was circumvented: for example, causing the system to violate its operators’ policies, make decisions unduly influenced by one user, or execute malicious instructions. This technique may be associated with additional attack techniques such as prompt injection, evasion, and model manipulation. 

<img width="373" alt="image" src="https://github.com/user-attachments/assets/6bebedcd-e5bd-4d1c-95d8-e544d17b41ab" />

![image](https://github.com/user-attachments/assets/f0f9e10d-0986-443e-9701-606467939d64)


### Crescendo attack

Here is an example of an attempt to ask an AI assistant to provide information about how to build a Molotov cocktail (firebomb). We know this knowledge is built into most of the generative AI models available today, but is prevented from being provided to the user through filters and other techniques to deny this request. Using a technique like Crescendo, however, the AI assistant can produce the harmful content that should otherwise have been avoided. This particular problem has since been addressed in Microsoft’s safety filters; however, AI models are still susceptible to it. Many variations of these attempts are discovered on a regular basis, then tested and mitigated.

![image](https://github.com/user-attachments/assets/2f2da3d6-2fff-45e6-b75b-a33418e0fe22)

### Dan

![image](https://github.com/user-attachments/assets/40209dcf-17e2-4d6f-a595-97182cd3edea)

### Skeleton key

![image](https://github.com/user-attachments/assets/5c1289da-5aad-4238-8ffe-7b35b62bc250)
![image](https://github.com/user-attachments/assets/5d86a407-07a5-406a-82e5-16daa89eea7a)

## Why is generative AI susceptible to this issue?
When integrating AI into your applications, consider the characteristics of AI and how they might impact the results and decisions made by this technology. Without anthropomorphizing AI, the interactions are very similar to the issues you might find when dealing with people. You can consider the attributes of an AI language model to be similar to an eager but inexperienced employee trying to help your other employees with their productivity:

- Over-confident: They may confidently present ideas or solutions that sound impressive but are not grounded in reality, like an overenthusiastic rookie who hasn’t learned to distinguish between fiction and fact.
- Gullible: They can be easily influenced by how tasks are assigned or how questions are asked, much like a naïve employee who takes instructions too literally or is swayed by the suggestions of others.
- Wants to impress: While they generally follow company policies, they can be persuaded to bend the rules or bypass safeguards when pressured or manipulated, like an employee who may cut corners when tempted.
- Lack of real-world application: Despite their extensive knowledge, they may struggle to apply it effectively in real-world situations, like a new hire who has studied the theory but may lack practical experience and common sense.

In essence, AI language models can be likened to employees who are enthusiastic and knowledgeable but lack the judgment, context understanding, and adherence to boundaries that come with experience and maturity in a business setting.

So we can say that generative AI models and system have the following characteristics:
- Imaginative but sometimes unreliable
- Suggestible and literal-minded, without appropriate guidance
- Persuadable and potentially exploitable
- Knowledgeable yet impractical for some scenarios

Without the proper protections in place, these systems can not only produce harmful content, but could also carry out unwanted actions and leak sensitive information.

## What is the scope of the problem?
When an AI jailbreak occurs, the severity of the impact is determined by the guardrail that it circumvented. Your response to the issue will depend on the specific situation and if the jailbreak can lead to unauthorized access to content or trigger automated actions. For example, if the harmful content is generated and presented back to a single user, this is an isolated incident that, while harmful, is limited. However, if the jailbreak could result in the system carrying out automated actions, or producing content that could be visible to more than the individual user, then this becomes a more severe incident. As a technique, jailbreaks should not have an incident severity of their own; rather, severities should depend on the consequence of the overall event (you can read about Microsoft’s approach in the AI bug bounty program).

Here are some examples of the types of risks that could occur from an AI jailbreak:
AI safety and security risks:
- Unauthorized data access
- Sensitive data exfiltration
- Model evasion
- Generating ransomware
- Circumventing individual policies or compliance systems
Responsible AI risks:
- Producing content that violates policies (e.g., harmful, offensive, or violent content)
- Access to dangerous capabilities of the model (e.g., producing actionable instructions for dangerous or criminal activity)
- Subversion of decision-making systems (e.g., making a loan application or hiring system produce attacker-controlled decisions)
- Causing the system to misbehave in a newsworthy and screenshot-able way
- IP infringement


## How do AI jailbreaks occur?

The two basic families of jailbreak depend on who is doing them:

A “classic” jailbreak happens when an authorized operator of the system crafts jailbreak inputs in order to extend their own powers over the system.
Indirect prompt injection happens when a system processes data controlled by a third party (e.g., analyzing incoming emails or documents editable by someone other than the operator) who inserts a malicious payload into that data, which then leads to a jailbreak of the system.
You can learn more about both of these types of jailbreaks here.

There is a wide range of known jailbreak-like attacks. Some of them (like DAN) work by adding instructions to a single user input, while others (like Crescendo) act over several turns, gradually shifting the conversation to a particular end. Jailbreaks may use very “human” techniques such as social psychology, effectively sweet-talking the system into bypassing safeguards, or very “artificial” techniques that inject strings with no obvious human meaning, but which nonetheless could confuse AI systems. Jailbreaks should not, therefore, be regarded as a single technique, but as a group of methodologies in which a guardrail can be talked around by an appropriately crafted input.
