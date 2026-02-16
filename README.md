# 🤖 Synaptic - Assistente IA para WhatsApp

Chatbot inteligente para WhatsApp com suporte a voz e texto.
Usa GPT-4 para respostas inteligentes e Whisper para transcrição de áudio.

## ✨ Funcionalidades

- 🎤 **Transcrição de voz** — Whisper (Groq + OpenAI fallback)
- 🧠 **IA Conversacional** — GPT-4o-mini com contexto de conversa
- 🔊 **Resposta em áudio** — Text-to-Speech via Edge TTS
- 📋 **Menu interativo** — Fluxo guiado + conversa livre
- 🔄 **Auto-reconexão** — Multi-device auth persistente
- ⌨️ **Indicadores naturais** — "digitando..." e "gravando..."
## 🏗️ Arquitetura
┌──────────────┐     ┌──────────────┐     ┌──────────────┐
│   WhatsApp   │◄───►│  Synaptic    │◄───►│  OpenAI API  │
│   (Baileys)  │     │  (Node.js)   │     │  (GPT-4)     │
└──────────────┘     └──────┬───────┘     └──────────────┘
│
┌──────┴───────┐
│   Groq API   │
│  (Whisper)   │
└──────────────┘

## ⚙️ Stack

- **Runtime:** Node.js
- **WhatsApp:** @whiskeysockets/baileys
- **IA:** OpenAI GPT-4o-mini
- **Voz:** Groq Whisper + Edge TTS
- **QR Code:** qrcode-terminal

## 🚀 Como Usar

1. Clone o repositório
2. Instale dependências:
```bash
npm install
```
3. Crie `.env` com suas credenciais:
```bash
OPENAI_API_KEY=sua_key
GROQ_API_KEY=sua_key
EMAIL_CONTATO=seu@email.com
```
4. Execute:
```bash
node index.js
```
5. Escaneie o QR Code com seu WhatsApp

## 📄 Licença

MIT License

## 👤 Autor

**Mário Marques De Goes**
- LinkedIn: [linkedin.com/in/seu-perfil](https://linkedin.com/in/mariomarques1987)
- Email: mariomarques1987@outlook.com
