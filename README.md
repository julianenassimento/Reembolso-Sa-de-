# ❤️ Reembolso Saúde +  
### Motor Inteligente de Triagem e Decisão Assistida em Reembolsos de Saúde

---

## 📌 Sobre o Projeto

O **Reembolso Saúde +** é um protótipo de assistente inteligente para pré-análise de pedidos de reembolso em planos de saúde.

O projeto combina:

- 🤖 IA Generativa para interpretação de linguagem natural  
- ⚙️ Motor determinístico de regras contratuais  
- 📊 Score explicável de confiança  
- 🔄 Classificação operacional automática  
- 🧠 Simulação de autoexecução inspirada em smart contracts  

A solução foi desenvolvida como projeto final do Bootcamp GenAI & Dados, aplicando conceitos de IA, Python, experiência do usuário e modelagem de decisão.

---

## 🎯 Problema

Processos de reembolso frequentemente enfrentam:

- Alto volume operacional  
- Retrabalho por documentação incompleta  
- Falta de previsibilidade para o cliente  
- Tempo médio de análise elevado  

O projeto propõe um motor híbrido capaz de:

- Interpretar automaticamente pedidos em linguagem natural  
- Simular valor estimado de reembolso  
- Avaliar completude documental  
- Classificar nível de complexidade  
- Indicar potencial de autoexecução supervisionada  

---

## 🧠 Arquitetura da Solução

A arquitetura é dividida em cinco camadas:

### 1️⃣ Camada de Interpretação (LLM)
Utiliza IA generativa para extrair dados estruturados a partir do texto do usuário.

Saída estruturada em JSON:
- Tipo de procedimento  
- Valor pago  
- Documentos informados  
- Tipo de plano  

---

### 2️⃣ Motor de Regras Determinísticas
Aplica regras contratuais mockadas:

Essa camada garante previsibilidade e explicabilidade.

---

### 3️⃣ Score de Confiança (0–100)

O score considera:

- Procedimento coberto  
- Valor dentro do limite  
- Documentação apresentada  
- Ausência de exceções contratuais  

Classificação:

| Score | Classificação Operacional |
|-------|---------------------------|
| ≥ 90  | Nível 2 – Autoexecução Supervisionada |
| 60–89 | Nível 1 – Revisão Simplificada |
| < 60  | Nível 0 – Auditoria Técnica |

---

### 4️⃣ Smart Rule Engine (Inspirado em Smart Contracts)

Inspirado no conceito de contratos autoexecutáveis, o sistema simula liberação automática condicional para casos de baixa complexidade.

⚠️ Importante:  
A decisão final sempre depende de validação sistêmica ou humana.

---

### 5️⃣ Explicabilidade

O sistema fornece justificativa clara para:

- Valor calculado  
- Limitações contratuais  
- Motivo da classificação  
- Nível de risco operacional  

---

## 🚀 Tecnologias Utilizadas

- Python  
- Streamlit  
- OpenAI API  
- Pydantic  
- JSON (modelagem de regras)  

---

## 📁 Estrutura do Projeto

reembolso-saude-plus/
│
├── app.py
├── requirements.txt
├── README.md
│
├── config/
│ └── rules.json
│
├── engine/
│ ├── rule_engine.py
│ ├── scoring.py
│ ├── classifier.py
│ └── autoexec.py
│
├── llm/
│ └── extractor.py
│
├── models/
│ └── request_model.py
│
├── utils/
│ └── helpers.py
│
└── data/
└── mock_plans.json


---

## 📊 Impacto Operacional Simulado

Cenário hipotético:

- 40% dos pedidos são de baixa complexidade  
- 70% desses atingem score ≥ 90  

Potencial impacto:

- Redução significativa do tempo médio de análise  
- Diminuição de retrabalho  
- Maior previsibilidade ao beneficiário  
- Liberação de analistas para casos complexos  

---

## 🛡 Governança e Limitações

- Projeto educacional e demonstrativo  
- Não utiliza dados reais  
- Não armazena informações pessoais  
- Não substitui decisão humana  
- Regras contratuais simuladas  

O objetivo é demonstrar arquitetura de decisão híbrida e eficiência operacional, não replicar sistema produtivo real.

---

## 🔮 Evoluções Futuras

- Integração com OCR para leitura automática de notas fiscais  
- Classificação automática de risco  
- Dashboard de métricas operacionais  
- Integração com APIs de pagamento  
- Modelagem preditiva de tempo médio de análise  

---

## 👩🏻‍💻 Autora

Juliane Nascimento  
Projeto desenvolvido no Bootcamp GenAI & Dados.

---

## 📎 Licença

Projeto para fins educacionais.
