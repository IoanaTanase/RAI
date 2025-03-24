# AI Mitigations
This is a list of common mitigations and scenarios based on the type of (generative) AI risk. 

## Harmful code 

Can apply to (not exhaustive):
- code generation

Potential mitigations (not exhaustive):
- Custom testing: https://learn.microsoft.com/en-us/azure/ai-services/content-safety/concepts/custom-categories?tabs=standard 
- UI / UX disclosures
  
## Harmful content

Can apply to (no exhaustive):
 - system that product content (both grounded and ungrounded)
 - single turn and multi turn chats
 - QA
 - rewrite
 - summarization
   
Potential mitigations (not exhaustive):
- Safety system message: https://github.com/IoanaTanase/RAI/blob/main/Safety%20System%20Messages/Harmful%20content.md
- Content filtering: https://learn.microsoft.com/en-us/azure/ai-foundry/concepts/content-filtering
- Blocklist: https://learn.microsoft.com/en-us/azure/ai-services/content-safety/how-to/use-blocklist?tabs=windows%2Crest
- UI / UX disclosures
  
## Jailbreaks

Can apply to (not exhaustive):
- content generation (grounded and ungrounded)
- single turn and multi turn chats
- QA
- rewrite
- summarization
- code generation

Potential mitigations (not exhaustive):
- Safety system message
- Prompt shields: https://learn.microsoft.com/en-us/azure/ai-services/content-safety/concepts/jailbreak-detection
- UI / UX disclosures
- Prompt filtering: https://learn.microsoft.com/en-gb/azure/ai-services/content-safety/concepts/jailbreak-detection
- Identity management: https://learn.microsoft.com/en-gb/entra/identity/managed-identities-azure-resources/overview
- Data access and controls: https://learn.microsoft.com/en-gb/purview/ai-microsoft-purview
- Content filtering: https://learn.microsoft.com/en-gb/azure/ai-services/openai/concepts/content-filter?tabs=warning%2Cuser-prompt%2Cpython-new
- Abuse monitoring: https://learn.microsoft.com/en-gb/azure/ai-services/openai/concepts/abuse-monitoring
- Model alignment and training: https://learn.microsoft.com/en-gb/training/paths/introduction-generative-ai/
- Threat protection: https://learn.microsoft.com/en-gb/azure/defender-for-cloud/ai-threat-protection
  
## Prompt injection attacks 

Can apply to (not exhaustive):
- content generation (grounded and ungrounded)
- single turn and multi turn chats
- QA
- rewrite
- summarization
- code generation
- Safety system message

Potential mitigations (not exhaustive):
- Safety system message: https://github.com/IoanaTanase/RAI/blob/main/Safety%20System%20Messages/Prompt%20injection%20attacks.md
- Prompt shields: https://learn.microsoft.com/en-us/azure/ai-services/content-safety/concepts/jailbreak-detection
  
## Ungrounded content (hallucinations)

Can apply to (not exhaustive)
- content generation (grounded)
- single and multi turn chats
- QA
- rewrite
- summarization
- code genertion (grounded)

Potential mitigations (not exhaustive):
- Safety system message: https://github.com/IoanaTanase/RAI/blob/main/Safety%20System%20Messages/%20Ungrounded%20content.md
- Groundness detection: https://learn.microsoft.com/en-us/azure/ai-services/content-safety/concepts/groundedness
- UI / UX disclosures
- Claimify: Extracting high-quality claims from language model outputs: https://www.microsoft.com/en-us/research/blog/claimify-extracting-high-quality-claims-from-language-model-outputs/

## IP infringement 

Can appply to (not exhaustive):
- content generation (typically ungrounded)
- single turn and multi turn chat

Potential mitigations (not exhaustive):
- Safety system message: https://github.com/IoanaTanase/RAI/blob/main/Safety%20System%20Messages/%20IP%20infringement.md
- UI / UX disclosures

## Manipulation and human-like behaviour 

Can apply to (not exhaustive)
- content generation (grounded)
- single and multi turn chats
- QA
- rewrite
- summarization

Potential mitigations (not exhaustive):
- Safety system message
- UI / UX disclosures

## Under and over reliance 

Can apply to (not exhaustive)
- content generation (grounded)
- single and multi turn chats
- QA
- rewrite
- summarization
- code generation

Potential mitigations (not exhaustive):
- Safety system message
- UI / UX disclosures and other: [https://github.com/IoanaTanase/RAI/blob/main/Safety%20System%20Messages/Reliance.md](https://github.com/IoanaTanase/RAI/blob/main/Measurement%20and%20Mitigations%20/Reliance.md)
