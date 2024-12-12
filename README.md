# AI English Tutor
아래 내용은 Byeongjin Kang님( https://github.com/jasonkang14 ) GitHub에서 ai-english-tutor( https://github.com/jasonkang14/ai-english-tutor/tree/main ) 내용에 대해 일부 수정을 가해서 교육용으로 사용하기 위해 다시 여기에 올렸습니다.

변경 내용은,
1. Mac 상에서 사용되는 필요 파이썬 라이브러리를 Windows PC용으로 변경하였고( requirements.txt 참조), 
2. Python 가상환경 venv 사용으로 다른 프로그램과 라이브러리 충돌이 생기지 않도록 했으며 
3. 에러가 발생하는 부분에 대해 고쳤습니다.
- 그리고 윈도우 PC 기준으로 되어있는 명령어는 리눅스 등에서는 역슬래시를 슬래시로 변경하는 등이 필요합니다.

## Overview
This project is an AI-powered English tutor that leverages various OpenAI APIs to create an interactive learning experience. It combines the capabilities of Chat Completions, Whisper (Speech to Text), and Text-to-Speech (TTS) to facilitate an engaging and dynamic English learning environment.

## Features
- [Chat Completions](https://platform.openai.com/docs/guides/text-generation/chat-completions-api): Creates an interactive chat thread for text-based English tutoring.
- [Whisper API](https://platform.openai.com/docs/guides/speech-to-text/speech-to-text): Implements Speech to Text functionality, allowing users to speak and have their speech converted to text.
- [Text-to-Speech (TTS)](https://platform.openai.com/docs/guides/text-to-speech/text-to-speech): Converts the language model's responses into audio, enabling an auditory learning experience.

## Prerequisites
- OpenAI API keys for Chat Completions, Whisper, and TTS services.
- Python 3.6 or later.
- Jupyter Notebook.

## Installation
1. Clone the repository:

```bash
git clone git@github.com/wemobile/ai-english-tutor.git
cd ai-english-tutor
.\aitutor\Scripts\activate
```
- 차후 Python 가상환경을 종료(또는 다른 가상환경으로 이동)하기 위해서는 .\aitutor\Scripts\deactivate.bat 실행

2. Install required Python packages:
```bash
pip install -r requirements.txt
```

3. Setup OpenAI API keys:

Set your OpenAI API keys as environment variables and store it in `.env` as `OPENAI_API_KEY`

```
OPENAI_API_KEY=sk-M4BeOHJ...
```

## Running the Project

1. Launch Jupyter Notebook:
```bash
jupyter notebook
```

you can also use VS Code if you would like

2. Open the project notebook (e.g., ai_english_tutor.ipynb) in the Jupyter interface.
3. Run the cells in sequence, following any instructions provided within the notebook.

## Usage
- Interact with the chatbot via the Jupyter Notebook interface. Type your English queries or statements, and the chatbot will respond.
- Use a microphone for the Speech to Text feature, speaking in English. The Whisper API will transcribe your speech.
- Listen to the TTS audio responses from the language model for auditory learning and practice.

## Contributions
- Contributions to this project are welcome! Please refer to the contribution guidelines for more information.
