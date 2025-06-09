# AgenteJUS

from dotenv import load_dotenv
import os
from openai import OpenAI
from IPython.display import Markdown

# Carrega .env
load_dotenv()

# Inicializa os clientes
openai = OpenAI(api_key=os.getenv("OPENAI_API_KEY"))
groq = OpenAI(api_key=os.getenv("GROQ_API_KEY"), base_url="https://api.groq.com/openai/v1")

# === Tarefas distintas ===
task_groq = "Liste os requisitos legais para abrir uma empresa de tecnologia no Brasil."
task_openai = "Explique os principais pontos da LGPD que uma nova empresa precisa seguir."

# === Groq responde sobre requisitos legais empresariais ===
res_groq = groq.chat.completions.create(
    model="llama3-70b-8192",
    messages=[{"role": "user", "content": task_groq}]
)
resposta_groq = res_groq.choices[0].message.content

# === OpenAI responde sobre LGPD ===
res_openai = openai.chat.completions.create(
    model="gpt-4",
    messages=[{"role": "user", "content": task_openai}]
)
resposta_openai = res_openai.choices[0].message.content

# === Agente crítico combina e refina ===
critic_prompt = f"""
Você é um assistente jurídico. Aqui estão duas respostas para tópicos complementares:

1. **Requisitos para abrir empresa (Groq):**
{resposta_groq}

2. **LGPD para empresas (OpenAI):**
{resposta_openai}

Una as duas informações em um único parecer claro, coeso e juridicamente sólido. Fale com tom profissional e prático, como se estivesse orientando um empreendedor brasileiro.
"""

res_critic = openai.chat.completions.create(
    model="gpt-4",
    messages=[{"role": "user", "content": critic_prompt}]
)
resposta_final = res_critic.choices[0].message.content

# Exibe a resposta final
display(Markdown(f"### Parecer Jurídico Integrado:\n\n{resposta_final}"))
