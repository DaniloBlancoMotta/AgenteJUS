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

### Parecer Jurídico Integrado (exemplo gerado - Groq + OpenAi): 

Ao iniciar uma nova empresa de tecnologia no Brasil, é essencial se familiarizar com os requisitos legais que regem tanto a criação da empresa quanto a gestão dos dados de seus clientes. Primeiramente, a escolha do tipo de empresa e o registro da mesma na Junta Comercial do Estado (JUCE) ou no Registro Civil das Pessoas Jurídicas (RCPJ) é crucial. Também é importante obter a Carteira de Pessoa Jurídica (CPJ) ou o Cadastro Nacional de Pessoa Jurídica (CNPJ) para a sua empresa.

As licenças e autorizações necessárias, como a Licença Municipal de Funcionamento (LMF), Licença de Atividade Econômica (LAE) e a Autorização de funcionamento pela Vigilância Sanitária (VISA) também devem ser consideradas. A empresa precisa estar cadastrada no Cadastro Nacional de Pessoas Jurídicas (CNPJ), Cadastro de Contribuintes do Estado (CADE) e Cadastro de Pessoas Físicas e Jurídicas (CPF/CNPJ).

É importante enfatizar que a contratação de funcionários deve seguir as leis trabalhistas, incluindo a assinatura de carteira de trabalho e o pagamento de impostos e contribuições sociais. A empresa também deve estar inscrita no cadastro de empregadores do Ministério do Trabalho (MTE).

Relativamente à propriedade intelectual, a empresa deve registrar seu software, marcas e domínios de internet nos respectivos órgãos. Além disso, diversas obrigações fiscais devem ser consideradas, como o pagamento de Imposto de Renda das Pessoas Jurídicas (IRPJ), Imposto sobre Serviços de Qualquer Natureza (ISSQN), a Contribuição para o Fundo de Garantia do Tempo de Serviço (FGTS) e a Contribuição para o Instituto Nacional do Seguro Social (INSS).

No que diz respeito à Lei Geral de Proteção de Dados (LGPD), a empresa deve obter o consentimento expresso do titular dos dados antes de coletar e processar os dados pessoais, além de operar de maneira transparente e minimizando a coleta de dados. Os dados podem ser coletados apenas para finalidades específicas, e a empresa deve garantir a segurança dos dados coletados. Em caso de violação de dados, a Autoridade Nacional de Proteção de Dados (ANPD) e o titular dos dados devem ser notificados. É necessário também nomear um encarregado para intermediar a comunicação entre a controladora de dados, os titulares dos dados e a ANPD.

Garantir todos esses pontos é crucial para evitar penalizações legais e garantir o sucesso da empresa. A orientação profissional de um advogado, contador ou consultor especializado em gestão de tecnologia pode ser crucial para uma implementação efetiva de todos os requisitos legais.
