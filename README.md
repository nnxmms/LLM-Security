# LLM-Security

> A Security Testing Suite for Large Language Models

## Introduction
LLM-Security is my personal security benchmark for testing large language models. It contains various exploits which make the models behave maliciously. 

> [!WARNING]  
> This collection is intended for educational purposes only. Do NOT use it for illegal activities.

## Getting Started
To get started with LLM-Security, follow these steps:

1. Clone the repository
```bash
git clone https://github.com/nnxmms/LLM-Security.git
```

2. Change directory to the downloaded repository
```bash
cd LLM-Security
```

3. Create a virtual environment
```bash
virtualenv -p python3.11 env
```

4. Activate the environment
```bash
source ./env/bin/activate
```

5. Install requirements
```bash
pip install -r requirements.txt
```

6. Register at [OpenAI](https://openai.com) to obtain a `OPENAI_API_KEY`

7. Create a `.env` file and update the values
```bash
cp .env.example .env
```

## Usage
Now you can run the benchmark with the following command
```bash
python3 benchmark.py
```
The results will be stored in a `benchmark.json` file

### OpenAI Example .env
```yaml
# General
VENDOR=openai
MODELNAME=gpt-3.5-turbo

# OpenAI
OPENAI_API_KEY=sk-...
```

### Ollama Example .env
```yaml
# General
VENDOR=ollama
MODELNAME=llama3:instruct

# OpenAI
OPENAI_API_KEY=
```

## Exploits
This table provides an overview of all exploits that are used within this benchmark.

| Paper | Link |
|---    |---   |
| Scalable and Transferable Black-Box Jailbreaks for Language Models via Persona Modulation | [Hacking and Security - Persona Modulatoin](https://hacking-and-security.cc/scalable-and-transferable-black-box-jailbreaks-for-language-models-via-persona-modulation/) |
| ArtPrompt: ASCII Art-based Jailbreak Attacks against Aligned LLMs                         | [Hacking and Security - ArtPrompt](https://hacking-and-security.cc/artprompt-ascii-art-based-jailbreak-attacks-against-aligned-llms/)                                   |
