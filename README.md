# Preoperative Fasting & Medication Adjustment Chatbot

This chatbot helps patients in Nova Scotia prepare for surgery by providing **accurate fasting times** and **safe medication adjustment guidance** based on trusted local and national medical guidelines.  
It uses a **Retrieval‑Augmented Generation (RAG)** pipeline powered by **AnythingLLM** and a local model via **Ollama**.

> ⚠️ **Disclaimer:** This chatbot does **not** provide professional medical advice or diagnoses. It is intended for educational use only. Always follow the specific instructions given by your surgical team. If you are experiencing a medical emergency, call 911 or visit the nearest emergency department.

---

## Project Overview

* **Scenario:** Pre‑Operative Fasting & Medication Adjustment Guidance  
* **Goal:** Build a domain‑specific chatbot that:
  * Delivers accurate fasting instructions tailored to surgery time.
  * Provides clear guidance on adjusting regular medications before surgery.
  * Cites **Nova Scotia Health** and **Canadian Anesthesiologists’ Society (CAS)** guidelines in each response.
  * Includes ethical safeguards and medical disclaimers in every answer.

---

## Tech Stack

| Layer           | Tool                                              | Role                                  |
| --------------- | ------------------------------------------------- | ------------------------------------- |
| LLM Frontend    | AnythingLLM                                       | UI + RAG + Prompt Injection           |
| LLM Backend     | Ollama                                            | Local model engine                    |
| LLM Model       | LLaMA 3 (via Ollama)                              | Generates responses                   |
| Documents       | NS Health, CAS Guidelines                         | Knowledge Base                        |
| Dev Environment | VS Code + GitHub                                  | Authoring & Collaboration             |

---

## Folder Structure

```
/preop-chatbot
├── knowledge_base/
│   ├── knowledge_document_1.pdf
│   ├── knowledge_document_2.pdf
│   ├── knowledge_document_3.pdf
│   └── knowledge_document_4.pdf
├── prompt/
│   └── system_prompt.txt
├── documentation/
│   ├── scenario_pack.md
│   └── use_case_description.md
├── demo/
│   ├── demo_video.mp4
│   └── chat_transcript.txt
└── README.md
```

---

## Knowledge Base File Structure

```
/preop-chatbot
└── knowledge_base/
    ├── knowledge_document_1.pdf  ← Nova Scotia Health Pre‑Operative Fasting Guidelines
    ├── knowledge_document_2.pdf  ← Canadian Anesthesiologists’ Society Guidelines
    ├── knowledge_document_3.pdf  ← Nova Scotia Health Perioperative Medication Adjustment Chart
    └── knowledge_document_4.pdf  ← Case‑21 Scenario Pack (context only)
```

---

## Prompt Engineering

* **System Prompt** designed to:
  * You are a preoperative fasting and medication adjustment assistant for patients in Halifax, Nova Scotia.

  * Use only:
  * Nova Scotia Health Pre-Operative Fasting Guidelines (latest available version)
  * Nova Scotia Health Perioperative Medication Adjustment Chart
  * Canadian Anesthesiologists’ Society (CAS) Guidelines to the Practice of Anesthesia (latest available version)

 * Requirements:
 * 1. Base all answers strictly on the above documents. Cite the source(s) in every answer (e.g., "According to Nova Scotia Health..." or "CAS Guidelines state...").
 * 2. Keep answers concise, clear, and easy for a general patient to understand.
 * 3. Apply timing and instructions to the patient’s stated surgery time whenever possible.
 * 4. Always include this disclaimer: “This is not medical advice. Always follow your surgical team’s instructions.”
 * 5. If a user asks about urgent symptoms, distress, or emergencies, tell them to contact their healthcare provider or call local emergency services immediately.
 * 6. Do not speculate or provide information outside of the uploaded guidelines.
 * 7. If patient is anxious help them calm down and tell them to talk to their family for support.
 * Tone: Supportive, factual, and patient-friendly.

---

## Integration Workflow

1. **Install and launch Ollama**
   ```bash
   ollama pull llama3
   ollama run llama3
   ```
2. **Launch AnythingLLM Desktop App**
3. **Create workspace:** `PreopChatbot`
4. **Upload knowledge_base documents** into workspace
5. **Paste custom system prompt** into Chat Settings > System Prompt
6. **Connect Ollama as the LLM Provider**
   * Provider: `Ollama`
   * Model name: `llama3`
7. **Test chatbot** with required and scenario‑specific questions
8. **Save transcript + record demo video**

---

## Testing Questions

The bot was tested with:

> "Hi, I’m having surgery next week at 8 in the morning and I am a bit anxious about it. Can you tell me when I should stop eating and drinking the night before?"  
> "I also take insulin for my diabetes. What’s the safest way to handle that before my operation?"

Both answers were evaluated for:
- Accuracy against NS Health & CAS guidelines
- Citation of correct sources
- Inclusion of disclaimers

---

## Demo Video

* File: `/demo/demo_video.mp4`  
* Shows chatbot setup, document integration, and answers to core scenario questions.

---

## Author

**Ariza Mollick**  
Master of Business Analytics, Saint Mary’s University  
July 2025  
**ariza.mollick@smu.ca**
