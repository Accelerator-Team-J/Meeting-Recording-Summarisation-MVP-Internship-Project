# 📋 Meeting Recording Summarization

Welcome to **Meeting Recording Summarization**, an AWS-based data pipeline that automates the process of taking minutes from meetings by converting video files into summarized text.

---
## 🚀 Project Overview
This project simplifies the burden of manual note-taking by leveraging cloud technologies to process meeting videos. It's ideal for busy teams that want accurate and concise summaries of their discussions.

---

## 🧩 Architecture Overview
```
A[Video Upload to S3] --> B[AWS Lambda Trigger]
B --> C[Audio Extraction]
C --> D[AWS Transcribe - Speech-to-Text]
D --> E[Summarization Service (Comprehend/NLP)]
E --> F[Store Summarized Text in S3 / Notify User]
```

---

## 🛠 Tech Stack
- **Language:** Python
- **Cloud Platform:** AWS
  - S3
  - Lambda
  - Transcribe
  - Comprehend (or custom NLP)
  - SQS/SNS
- **Tools:** GitHub, Docker (optional), CI/CD (optional)

---

## 🔍 Features
- Automatically detects and processes uploaded video files.
- Converts audio to text using AWS Transcribe.
- Summarizes the transcribed content.
- Outputs a readable summary to storage or user inbox.

---

## 👩🏽‍💻 My Role
- Built Python scripts to interface with AWS Lambda.
- Set up and tested AWS Transcribe integration.
- Participated in designing and validating the end-to-end pipeline.
- Contributed to the summarization logic implementation.

---

## 📁 File Structure
```bash
meeting-recording-summarization/
├── lambda/
│   ├── transcribe_handler.py      # Handles transcription
│   └── summarize_handler.py       # Handles text summarization
├── utils/
│   ├── s3_helpers.py              # S3 upload/download helpers
│   └── audio_converter.py         # Extracts audio from video
├── README.md
└── architecture.png (optional visual)
```

---

## 📌 Future Enhancements
- Add language detection for multilingual support
- Implement streaming transcription
- Integrate with a front-end uploader

---

## 🤝 Contributions
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

---

## 📜 License
[MIT](https://choosealicense.com/licenses/mit/)

