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
