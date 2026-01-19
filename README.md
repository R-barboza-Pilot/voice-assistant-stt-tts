# voice-assistant-stt-tts
Este projeto implementa um assistente conversacional por voz, capaz de compreender perguntas feitas por áudio e responder de forma falada.

Você pode copiar e colar direto no GitHub.

# 🎙️ Assistente Conversacional por Voz com Whisper, ChatGPT e gTTS

## 📌 Descrição do Projeto
Este projeto implementa um **assistente conversacional por voz**, capaz de compreender perguntas feitas por áudio e responder de forma falada. A solução integra tecnologias de **Speech-to-Text (STT)** e **Text-to-Speech (TTS)** em sinergia com **Inteligência Artificial Generativa**, permitindo interações naturais e multi-idiomas.

O sistema utiliza o **Whisper**, da OpenAI, para transcrição automática de fala, o **ChatGPT** para geração de respostas inteligentes e o **Google Text-to-Speech (gTTS)** para converter texto em áudio.

Este projeto foi desenvolvido como parte de um **desafio prático da DIO**, com foco em aplicação real, boas práticas e organização de código.

---

## 🧠 Arquitetura da Solução

O fluxo da aplicação segue o pipeline abaixo:



🎤 Microfone
↓
📝 Whisper (Speech-to-Text)
↓
🤖 ChatGPT (OpenAI API)
↓
🔊 gTTS (Text-to-Speech)
↓
🔈 Usuário


Cada etapa é desacoplada em módulos específicos, facilitando manutenção, testes e futuras evoluções.

---

## 🛠️ Tecnologias Utilizadas
- **Python**
- **OpenAI API**
  - Whisper (Speech-to-Text)
  - ChatGPT (IA Generativa)
- **Google Text-to-Speech (gTTS)**
- **sounddevice** (captura de áudio)
- **scipy** (manipulação de arquivos WAV)
- **playsound** (reprodução de áudio)
- **python-dotenv** (variáveis de ambiente)

---

## 📂 Estrutura do Projeto

voice-chatgpt/
│
├── src/
│ ├── audio_input.py # Captura de áudio do microfone
│ ├── speech_to_text.py # Transcrição com Whisper
│ ├── chatgpt_client.py # Comunicação com ChatGPT
│ ├── text_to_speech.py # Conversão de texto em áudio
│ └── main.py # Orquestração do fluxo
│
├── audio/
│ ├── input.wav
│ └── output.mp3
│
├── .env.example
├── requirements.txt
└── README.md

---

## ⚙️ Como Executar o Projeto

### 1️⃣ Clonar o repositório
bash
git clone https://github.com/seu-usuario/voice-chatgpt
cd voice-chatgpt

2️⃣ Criar e ativar ambiente virtual (opcional)
python -m venv venv
source venv/bin/activate  # Linux/Mac
venv\Scripts\activate     # Windows

3️⃣ Instalar as dependências
pip install -r requirements.txt

4️⃣ Configurar variáveis de ambiente

Crie um arquivo .env baseado no .env.example:

OPENAI_API_KEY=sua_chave_da_openai

5️⃣ Executar a aplicação
python src/main.py

▶️ Exemplo de Uso

O sistema grava a voz do usuário por alguns segundos.

O áudio é transcrito automaticamente pelo Whisper.

O texto é enviado ao ChatGPT.

A resposta gerada é convertida em áudio.

O usuário escuta a resposta falada.

Exemplo:

Usuário: "Qual é a capital da França?"
Assistente: "A capital da França é Paris." 🔊

🌍 Funcionalidades

🎤 Captura de áudio via microfone

📝 Transcrição automática de fala

🤖 Respostas inteligentes com IA generativa

🔊 Conversão de texto em voz

🌐 Suporte a múltiplos idiomas (via Whisper e gTTS)

🚀 Possíveis Evoluções

Detecção automática de idioma para o TTS

Conversação contínua (loop)

Memória de contexto da conversa

Interface gráfica ou web

Detecção de silêncio no áudio

Deploy em nuvem

🎓 Aprendizados

Com este projeto foi possível consolidar conhecimentos em:

Integração de APIs de IA

Processamento de áudio em Python

Arquitetura modular

Boas práticas de organização de projetos

Desenvolvimento de soluções baseadas em IA generativa


