# Hi, I'm Joe

Final-year Computer and Communication Engineering student (AI option) at Saint Joseph University of Beirut (USJ), graduating in May 2027. I build machine-learning models and LLM-powered applications and take them through to deployment.

## Skills

- **Languages:** Python, Java, C++
- **Machine learning:** scikit-learn, PyTorch, XGBoost, LightGBM, SMOTE, Optuna, Pandas, NumPy
- **LLMs and agents:** Gemini API, Groq, Ollama, Qwen, Model Context Protocol (MCP), prompt engineering, structured JSON outputs, RAG
- **Speech and vision:** Whisper, edge-tts, YOLOv5, CLIP, MediaPipe
- **Backend and deployment:** Flask, FastAPI, REST APIs, MongoDB, Docker, Vercel, Hugging Face Spaces
- **Tools:** n8n, Git, Linux, Jupyter

## Featured projects

### ETIB Interpreter Trainer · Deployed

 [Repository](https://github.com/joe-haddad3/etib-interpreter-trainer)

A web platform used by interpreting students at USJ's School of Translators and Interpreters (ETIB). It generates practice speeches with an LLM, reads them aloud in 21 voices across Arabic, French and English, transcribes the student's interpretation with Whisper, and returns an evaluation of hesitations, omissions, number errors and terminology.

- Built during a summer 2026 internship in a team of six, with ETIB as the client
- One Gemini call returns the speech, summary, quiz and trilingual glossary as structured JSON
- Speeches can be grounded in UN documents through a RAG pipeline
- Python, Flask, React, Gemini, Groq Whisper, MongoDB, Docker

### IoT Intrusion Detection · Completed

[Repository](https://github.com/joe-haddad3/iot-intrusion-detection) 

Classifies IoT network traffic from the CIC IoT 2023 dataset (2.9M training samples) and serves predictions through a FastAPI service with drift monitoring. We compared 8 models, from logistic regression to a stacking ensemble, and handled heavy class imbalance with SMOTE and class weighting.

- **Multiclass, 34 classes (33 attack types + benign):** macro-F1 0.648, accuracy 79.9% (LightGBM + SMOTE, tuned with Optuna)
- **Binary, benign vs attack:** F1 0.973, ROC-AUC 0.983, accuracy 94.9% (LightGBM)
- Group project with Charbel Eid and Elie Saddy · Python, scikit-learn, LightGBM, XGBoost, PyTorch, FastAPI, Docker

### AI Penetration Testing Agent · Experimental

A local LLM (Qwen 2.5 14B via Ollama) connected to security tools on Kali Linux through MCP, running fully offline in an isolated lab with human approval for every action. *Code not public yet.*

### AI Medical Article Detector · Completed

An n8n workflow that collects new medical research daily, checks each article with rule-based heuristics and the Groq LLM, and flags likely AI-generated content in a dashboard and daily email report. *Code not public yet.*

### Other projects

- **[Robot Bodyguard](https://github.com/joe-haddad3/robot-bodyguard):** security robot with YOLOv5 person and weapon detection, CLIP + FaceNet owner recognition and MediaPipe behaviour analysis on Raspberry Pi 5. Group project with Charbel Eid.
- **[DriverGuard](https://github.com/joe-haddad3/DriverGuard-):** webcam driver monitoring for drowsiness, yawning, head tilt and phone use. Course project built with a classmate.

## Experience

**AI Engineering Intern**, USJ (ESIB · ETIB · CINIA) · Jun – Jul 2026

Built and deployed the ETIB Interpreter Trainer with a team of six: LLM integration, prompt design from ten client requirements, and checking the generated glossary against UN and EU terminology databases.

**Intern**, Ingram Micro Levant · Aug 2026

Rotation across infrastructure, cybersecurity, networking and presales teams, with hands-on labs in network architecture and security.

## Contact

[LinkedIn](https://www.linkedin.com/in/joe-haddad34/) · [CV (PDF)](Joe%20Haddad%20CV.pdf) . joe.haddad2@outlook.com
