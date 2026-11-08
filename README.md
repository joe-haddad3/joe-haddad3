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

### AI Penetration Testing Agent · Completed

[Repository](https://github.com/joe-haddad3/hexstrike-ai-local-llm)

A local LLM (Qwen 2.5 14B via Ollama) drives the HexStrike AI MCP server, which gives it access to 150+ security tools on Kali Linux. Everything runs offline in an isolated lab, and every command needs human approval. We built two integrations: a small REST bridge, and the MCP path through ollmcp, which needed a compatibility patch for the MCP v2 library.

- On a Metasploitable 3 lab machine, the model chained nmap, enum4linux, gobuster, nikto and hydra by itself and found 9 open services, an exposed Drupal site and weak SSH credentials
- A 14B model struggled with 150 tools; limiting it to the few tools needed made its tool calls reliable
- Ethical-hacking course project with Georges El Hajj · Python, Ollama, Qwen 2.5, MCP, Kali Linux

### AI Medical Article Detector · Completed

[Repository](https://github.com/joe-haddad3/ai-medical-article-detector)

An n8n workflow that estimates how likely medical articles are to be AI-written. Every morning it collects new articles from PubMed, Zenodo and Europe PMC, scores each one with a rule-based detector and an LLM judge on Groq, emails a report and publishes the results as JSON for a website. A second lane scans PDF or DOCX files sent by email and replies with a score.

- Rule-based scorer with no API calls: AI "tell" words, stock phrases, sentence-length variation, and credit for concrete statistics
- If the LLM call fails, articles keep their rule score and the report says so, instead of silently reporting zero flagged articles
- n8n, Groq (gpt-oss-120b), REST APIs, Gmail SMTP/IMAP, GitHub API

### Other projects

- **[Robot Bodyguard](https://github.com/joe-haddad3/robot-bodyguard):** security robot with YOLOv5 person and weapon detection, CLIP + FaceNet owner recognition and MediaPipe behaviour analysis on Raspberry Pi 5. Group project with Charbel Eid.

## Experience

**AI Engineering Intern**, USJ (ESIB · ETIB · CINIA) · Jun – Jul 2026

Built and deployed the ETIB Interpreter Trainer with a team of six: LLM integration, prompt design from ten client requirements, and checking the generated glossary against UN and EU terminology databases.

**Intern**, Ingram Micro Levant · Aug 2026

Rotation across infrastructure, cybersecurity, networking and presales teams, with hands-on labs in network architecture and security.

## Contact

[LinkedIn](https://www.linkedin.com/in/joe-haddad34/) · [CV (PDF)](Joe%20Haddad%20CV.pdf) · [joe.haddad2@outlook.com](mailto:joe.haddad2@outlook.com)
