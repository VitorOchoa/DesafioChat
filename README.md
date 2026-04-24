# Projeto Bootcamp DIO - Assistente de Voz com IA

## 📌 Sobre o Projeto
Este projeto foi desenvolvido como parte de um bootcamp da [Digital Innovation One (DIO)](https://www.dio.me/).  
O objetivo é criar um fluxo completo de interação por voz utilizando **Google Colab**, **Whisper** para transcrição de áudio, **OpenAI GPT-4** para geração de respostas inteligentes e **gTTS** para síntese de voz.

## 🚀 Funcionalidades
- Gravação de áudio diretamente no Google Colab usando JavaScript.
- Transcrição automática do áudio com o modelo Whisper.
- Processamento da transcrição pelo modelo GPT-4 para gerar respostas inteligentes.
- Conversão da resposta em áudio com gTTS.
- Reprodução automática da resposta em voz no Colab.

## 🛠️ Tecnologias Utilizadas
- **Python 3**
- **Google Colab**
- **JavaScript (MediaStream Recording API)**
- **OpenAI Whisper**
- **OpenAI GPT-4**
- **gTTS (Google Text-to-Speech)**
- **IPython.display (para áudio e execução de JS)**

## 📂 Estrutura do Projeto
- `record()` → Função para gravar áudio do usuário.
- `whisper.transcribe()` → Transcreve o áudio gravado.
- `openai.ChatCompletion.create()` → Envia a transcrição para o GPT-4 e recebe a resposta.
- `gTTS()` → Converte a resposta em áudio.
- `Audio()` → Reproduz o áudio gerado.

## ▶️ Como Executar
1. Clone este repositório ou copie os arquivos para o Google Colab.
2. Configure sua chave da OpenAI:
   ```python
   import os
   os.environ['OPENAI_API_KEY'] = "sua_chave_aqui"
