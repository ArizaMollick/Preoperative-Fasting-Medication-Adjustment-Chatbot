# Scenario Pack: Preoperative Fasting and Medication Adjustment

## Scenario Background
In Halifax, Nova Scotia, patients scheduled for surgery must follow specific instructions about fasting (NPO
guidelines) and adjusting medications to reduce risks during anesthesia. Misunderstanding these instructions
can lead to surgery cancellations or complications. Nova Scotia Health and Canadian anesthesiology
organizations provide clear patient education materials on fasting times and medication management. This
scenario asks students to use the Ollama + AnythingLLM stack, combined with locally available, authoritative
health education materials, to design a chatbot for Preoperative Fasting and Medication Adjustment
Guidance.

## Scenario Goals
- Help users understand preoperative fasting (NPO) instructions  
- Guide users on safe adjustments to regular medications before surgery  
- Clearly communicate that the chatbot does not provide professional medical diagnoses and cannot
replace personalized instructions from surgical teams  

## Recommended Knowledge Base Materials
Students should collect and organize retrievable, structured local health education materials to serve as their
RAG knowledge base. Recommended sources include:
- Nova Scotia Health – Preoperative Fasting Guidelines  
- Canadian Anesthesiologists’ Society – Patient Instructions  
- Hospital Surgical Preparation Instructions  
- Medication Adjustment Charts for Surgery  
- Any relevant local clinic or hospital resources  

## Requirement
Upload as PDF, Markdown, or plain text, using general, consistent file names such as:
```
knowledge_document_1.pdf
knowledge_document_2.md
knowledge_document_3.txt
```

## Suggested User Questions for Testing
Your final system must be able to answer these scenario questions using your uploaded knowledge base
materials:
1. "My surgery is at 8 a.m.—when should I stop eating and drinking?"  
2. "Do I need to stop taking my aspirin before surgery?"  

## Suggested GitHub Repository Structure
```
📂 /cold-flu-chatbot 
├─ knowledge_base/ 
│  ├─ knowledge_document_1.pdf 
│  ├─ knowledge_document_2.md 
│  └─ knowledge_document_3.txt 
├─ prompt/ 
│  └─ system_prompt.txt 
├─ documentation/ 
│  └─ scenario_pack.md (Provided) 
│  └─ use_case_description.md 
├─ demo/ 
│  ├─ demo_video.mp4 
│  └─ chat_transcript.txt 
└─ README.md 
```

## Deliverables
**Knowledge Base**  
- Include all documents actually used in AnythingLLM  
- Must be clearly structured and named using the general format above  

**System Prompt**  
- Defines the chatbot role, tone, scope, and ethical disclaimers  

**Use Case Description**  
- A clear document that identifies user pain points and success criteria  

**Demo Materials**  
- Screen recording or video showing chatbot responses to the core scenario questions  
- Chat transcript  

**README.md**  
- Brief project overview  
- Local deployment/testing instructions  
- Author(s) and date  

## Important Notes
- The project is for educational research use only and must not be used for real diagnosis or treatment.  
- The chatbot README.md file must prominently display a “Not Medical Diagnosis” disclaimer.

