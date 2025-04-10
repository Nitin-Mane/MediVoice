
# MediVoice 🩺🧠

![Status](https://img.shields.io/badge/status-active-brightgreen)
![Python](https://img.shields.io/badge/python-3.8%2B-blue)
![License](https://img.shields.io/badge/license-MIT-lightgrey)
![Platform](https://img.shields.io/badge/platform-RaspberryPi%20%7C%20Linux%20%7C%20Cloud-orange)

> Real-time Clinical Voice Documentation and Decision Support using AI + Edge Computing + Agentic RAG

---

## 🧬 Overview

**MediVoice** is a research-driven, hackathon-born project aimed at enhancing **clinical documentation** in ICU and surgical ward environments. It captures real-time conversations between doctors and healthcare staff, recognizes speaker roles, detects alarm events, and generates structured patient summaries using AI. The goal is to reduce documentation fatigue, ensure medical audit traceability, and improve treatment workflows through intelligent automation.

---

## 💻 Features

- 🎙️ Real-time voice-to-text transcription with Whisper
- 🩺 Speaker diarization to identify Doctor/Nurse/Patient
- 🔊 Alarm sound detection using YAMNet/VGGish
- 🧠 Agentic RAG-based note generation using LLMs (BioGPT/MedPalm)
- ✍️ Grammar correction and sentence cleaning
- 🗂️ Compact clinical note generation
- 🧾 Knowledge graph formation based on patient-timeline-treatment

---

## 📊 Architecture

**Edge Device:** Raspberry Pi + Mic  
**Server:** Transcription + Summarization + NLP Inference  
**LLM Layer:** Agentic RAG + Clinical Note Prompts  
**Output:** Structured Notes (History, Exam) + Compact Summary

<p align="center">
  <img src="docs/assets/architecture.png" alt="MediVoice Architecture" width="600"/>
</p>

---

## 📁 Repository Structure

```bash
📦 MediVoice/
├── README.md
├── requirements.txt
├── inference/
│   ├── speaker_diarization.py
│   ├── whisper_transcription.py
│   ├── alarm_detection.py
├── rag_pipeline/
│   ├── summarizer.py
│   ├── prompt_templates.md
├── docs/
│   ├── architecture.md
│   ├── methodology.md
│   ├── sample_outputs.md
│   └── assets/
│       └── architecture.png
```

---

## 📄 Documentation

- [System Architecture](docs/architecture.md)
- [NLP + Summarization Methodology](docs/methodology.md)
- [Prompt Engineering Strategies](rag_pipeline/prompt_templates.md)
- [Sample Outputs](docs/sample_outputs.md)

---

## 🧪 Getting Started

```bash
# Clone the repo
git clone https://github.com/mnitin59/MediVoice.git
cd MediVoice

# Install dependencies
pip install -r requirements.txt

# Run a sample
python inference/whisper_transcription.py --input sample.wav
```

---

## 📌 Research Direction

This project is inspired by **multimodal LLM workflows** for medical summarization, **Bayesian network-based simulation pipelines**, and **real-time NLP deployment in edge environments**. It is being actively developed under the IIT Ropar x Harvard Hackathon 2025 and will contribute toward scalable AI integration in clinical documentation systems.

---

## 📚 Citation

```latex
@misc{mane2025medivoice,
  title={MediVoice: An AI-Powered Clinical Voice Documentation System with Agentic RAG},
  author={Nitin Mane et al.},
  year={2025},
  note={Hackathon project – IIT Ropar x Harvard},
}
```

---

## 🙏 Acknowledgments

Special thanks to our mentors, hackathon organizers, and the medical AI community for their support.

---

## 📬 Contact

Nitin Mane  \\
M.Tech Mechatronics, IIT Bhilai  \\
[LinkedIn](https://www.linkedin.com/in/nitingmane/) | [GitHub](https://github.com/Nitin-Mane)

Team Mates: 

