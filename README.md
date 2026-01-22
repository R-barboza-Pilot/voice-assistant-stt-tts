
# 🎙️ Voice Chat com Whisper (Python)

Projeto simples em Python que grava áudio do microfone e realiza transcrição usando o modelo Whisper da OpenAI.

Ideal para estudos de:
- Speech to Text (STT)
- Integração com APIs de IA
- Projetos iniciais com Python + OpenAI

---

## 🚀 Funcionalidades

- Grava áudio do microfone
- Salva em arquivo `.wav`
- Transcreve usando Whisper (OpenAI)
- Estrutura profissional de projeto
- Pronto para evoluir para ChatGPT + TTS

---

## 🛠️ Tecnologias utilizadas

- Python 3.10+
- OpenAI API
- Whisper
- SoundDevice
- SciPy
- VS Code

---

## 📁 Estrutura do projeto

voice-chatgpt-whisper/
├── src/
│ └── main.py
├── .env.example
├── .gitignore
├── requirements.txt
└── README.md

---

## ⚙️ Como executar o projeto

### 1️⃣ Clonar o repositório

git clone https://github.com/seu-usuario/voice-chatgpt-whisper.git
cd voice-chatgpt-whisper

2️⃣ Criar ambiente virtual
python -m venv venv

Ativar no Windows (PowerShell):

venv\Scripts\activate

3️⃣ Instalar dependências
pip install -r requirements.txt

4️⃣ Configurar variável de ambiente

Crie um arquivo .env baseado no exemplo:

OPENAI_API_KEY=sua_chave_aqui

5️⃣ Executar o projeto
python src/main.py

O sistema irá:

Gravar 5 segundos de áudio

Salvar o arquivo

Tentar transcrever (necessário crédito na OpenAI)

⚠️ Observações importantes

Se não houver crédito na OpenAI, o projeto exibirá erro 429 (quota) — isso é esperado.

O áudio ainda será gravado normalmente.

O arquivo venv/ não deve ser versionado.

📌 Próximos passos (evolução)

Integração com ChatGPT

Conversa por voz contínua

Text-to-Speech (TTS)

Interface gráfica

👨‍💻 Autor

Projeto desenvolvido para fins educacionais e estudo de IA aplicada.

## 🚀 Próximos passos

- Integração com ChatGPT
- Conversa por voz contínua
- Text-to-Speech (TTS)
- Interface gráfica


