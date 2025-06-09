# AgenteJUS 

# Legal Agent: Assistente Jurídico com Agentes LLM

Este projeto implementa um agente jurídico inteligente, que utiliza múltiplos modelos de linguagem (Groq + OpenAI) para oferecer pareceres jurídicos precisos e integrados. Ele aplica padrões de design agentic como _Parallel Task Decomposition_ e _Critic Evaluation_.

## ✨ Funcionalidades

- Consulta jurídica dividida por especialidade
- Avaliação crítica das respostas
- Resposta final coesa e explicativa
- Pronto para rodar localmente via Cursor, VS Code ou Jupyter

## 🧰 Tecnologias

- Python 3.10+
- OpenAI SDK
- Groq API (formato OpenAI-compatible)
- python-dotenv
- IPython / Markdown (para visualização)

## 🚀 Como usar

1. Clone o repositório
2. Crie um arquivo `.env` com suas chaves:
   ```bash
   cp .env.example .env

