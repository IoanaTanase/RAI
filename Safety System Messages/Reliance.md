Source: https://www.microsoft.com/en-us/research/uploads/prod/2024/03/GenAI_AppropriateReliance_Published2024-3-21.pdf

# Reliance 

**Appropriate reliance** on AI happens when users accept correct AI outputs and reject incorrect ones. 
It requires users of AI systems to know when to trust the AI and when to trust themselves. 

**Under-reliance** happens when users overestimate their own performance or underestimate the system performance, leading them to ignore correct system outputs (He et al., 2023). 

**Overreliance** happens when users either underestimate their own performance or overestimate the system performance, leading them to accept incorrect outputs (Passi &  Vorvoreanu, 2022).

<img width="502" alt="image" src="https://github.com/user-attachments/assets/32ae760d-7f1d-4c8f-b2d7-43ac1f3a591f" />

## When this concern might 

Should be considered for any system where the principle of "human in the loop" applies. The concept of "human-in-the-loop" (HITL) in AI systems refers to the integration of human oversight and intervention within the AI decision-making process. This approach ensures that human judgment and expertise are incorporated alongside machine intelligence.

## Considerations for components 

Like any other safety system message, these should be considered in conjunction with broader AI risk mitigation such as, but not limited to base model (and potential fine tunning), safety system mitigations (classifiers, block list etc), groundness / RAG and UI/UX (such as disclaimers etc).
Also not all the below components should be introduced at the same time, depending on the system's use case there are different options to choose from. 

### Both under- and over- reliance 

Components that instruct the model to include:
- **AI critiques**: explanations that provide evidence, descriptions, or solutions for specific flaws in AI outputs.
- **Contrastive explanations**: explanations that provide both evidence that supports as well as evidence that refutes an AI-generated claim.
- **Uncertainty expressions**: Uncertainty expressions can facilitate appropriate reliance by providing information about how likely it is that certain parts of GenAI outputs are right or wrong using numbers (e.g., confidence scores), visuals (e.g., color highlights), or language (e.g., hedging). 

### Under-reliance 

When under-reliance stems from ungrounded / hallucinated output, using groundness safety system components can increased quality of output and by association increase trust and usefulness of the system as  a whole. 

### Over-reliance 

Components that instruct the model to include:
- **Background information**: Although also a type of verification-focused explanation, background explanations differ by providing information outside the AI’s training data to facilitate verification of AI outputs




