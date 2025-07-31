# Use Case Description: Preoperative Fasting & Medication Adjustment Chatbot

## 1. Scenario Overview
This chatbot is designed to assist patients in Nova Scotia who are scheduled for surgery by providing clear, accurate, and guideline-based information about **preoperative fasting (NPO)** requirements and **medication adjustments**.  
The goal is to ensure patients understand when to stop eating and drinking before surgery and how to manage their regular medications, in alignment with official guidelines from Nova Scotia Health and the Canadian Anesthesiologists’ Society (CAS).

---

## 2. Target Users
- Patients in Nova Scotia scheduled for elective surgery.
- Especially those who:
  - Need clarity on fasting cut-off times based on their surgery schedule.
  - Require instructions on adjusting specific medications (e.g., aspirin, insulin).
  - Prefer straightforward, patient-friendly explanations.

---

## 3. User Pain Points
- **Confusion** about fasting instructions and timelines.
- **Uncertainty** about which medications to continue or stop.
- **Risk of surgery cancellation** due to incorrect preparation.
- **Difficulty finding accurate, localized information** quickly.

---

## 4. Goals and Success Criteria

### Goals:
1. Deliver accurate, guideline-aligned fasting instructions tailored to the patient’s surgery time.
2. Provide medication adjustment recommendations based on authoritative sources.
3. Include proper citations from **Nova Scotia Health** and **CAS** in each answer.
4. Always include the disclaimer: “This is not medical advice. Always follow your surgical team’s instructions.”
5. Redirect urgent or emergency cases to healthcare providers immediately.

### Success Criteria:
- Chatbot responses **match** Nova Scotia Health & CAS guidelines.
- Every answer includes **citation** + **disclaimer**.
- Responses are **concise, clear, and easy to follow**.
- No irrelevant or speculative information.

---

## 5. Ethical Considerations
- **Not a substitute for professional medical advice** — must always state this clearly.
- **No collection or storage** of personal health information.
- Crisis handling: refer patients in distress to contact their healthcare provider or call 911.
- Only answer within the scope of uploaded documents.

---

## 6. Knowledge Base Sources
1. **Nova Scotia Health – Pre‑Operative Fasting Guidelines (2025)**  
2. **Nova Scotia Health – Perioperative Medication Adjustment Chart (2025)**  
3. **Canadian Anesthesiologists’ Society – Guidelines to the Practice of Anesthesia (2025)**  
4. **Case 21 Scenario Pack** (for project context only)

---

## 7. Example User Questions
- “My surgery is at 8 a.m.—when should I stop eating and drinking?”
- “Do I need to stop taking my aspirin before surgery?”
- “Can I have coffee with milk before my procedure?”
- “I’m on insulin for diabetes. How should I manage it before surgery?”

---

## 8. Expected Output Format
1. **Citation** of source document(s).
2. **Main recommendation** in plain language.
3. **Adaptation** of timing or guidance to patient’s situation.
4. **Examples** (e.g., list of allowed clear fluids).
5. **Disclaimer** repeated in every answer.

---

## 9. Integration Testing Plan
The chatbot will be tested with:
1. “Hi, I’m having surgery next week at 8 in the morning and I am a bit anxious about it. Can you tell me when I should stop eating and drinking the night before?”
2. "I also take insulin for my diabetes. What’s the safest way to handle that before my operation?""

Responses will be evaluated for **accuracy**, **citations**, **clarity**, and **inclusion of disclaimers**.
