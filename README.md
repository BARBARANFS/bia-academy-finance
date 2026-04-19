# 💡 BIA Academy Finance


<p align="center">
  <img src="assets/imagens_readme/Logo.png" alt="BIA Academy Logo" width="200"/>
</p>



<p align="center">
  <b>BIA Academy Finance</b>
</p>

<p align="center">
  <b>Educadora Financeira Inclusiva com IA Local</b><br>
  <i>Aplicação de IA Generativa focada em educação financeira acessível, segura e personalizada</i>
</p>
>

<p align="center">
  <b>Educadora Financeira Inclusiva com IA Local</b><br>
  <i>Aplicação de IA Generativa focada em educação financeira acessível, segura e personalizada</i>
</p>

---

<p align="center">

![Python](https://img.shields.io/badge/Python-3.10%2B-blue?style=for-the-badge\&logo=python)
![Streamlit](https://img.shields.io/badge/Streamlit-App-red?style=for-the-badge\&logo=streamlit)
![AI](https://img.shields.io/badge/AI-Local-green?style=for-the-badge)
![RAG](https://img.shields.io/badge/RAG-Enabled-purple?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Concluído-success?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-lightgrey?style=for-the-badge)

</p>

---

## 🎯 Contexto do Projeto

Projeto desenvolvido no **Bootcamp Bradesco - GenAI & Dados** da DIO (Digital Innovation One).

O objetivo é aplicar conceitos de **IA Generativa**, **RAG** e **experiência inclusiva**, construindo um agente funcional com foco em impacto real.

---

## 🎥 Demonstração

<p align="center">
  <img src="assets/demo.gif" alt="Demonstração da BIA Academy" width="800"/>
</p>

🎧 **Teste de acessibilidade (áudio):**
👉 [https://BARBARANFS.github.io/bia-academy-finance/](https://BARBARANFS.github.io/bia-academy-finance/)

---

## 📌 Visão Geral

A **BIA Academy Finance** é uma aplicação de IA que atua como uma **educadora financeira inclusiva**, utilizando:

* IA **100% local (offline)**
* Base de conhecimento própria
* Sistema **RAG (busca contextual)**
* Adaptação por perfil de usuário
* Recursos de acessibilidade (áudio)

---

## ❌ Problema

A educação financeira ainda apresenta barreiras significativas:

* Linguagem excessivamente técnica
* Falta de acessibilidade
* Baixa personalização
* Dificuldade para iniciantes

---

## ✅ Solução

A BIA oferece uma experiência educativa baseada em:

* 💬 Chat inteligente com IA
* 🧠 Aprendizado ativo via quiz
* 🎮 Gamificação com jogo evolutivo
* 🎯 Adaptação por perfil
* 🔊 Acessibilidade por áudio
* 🔐 Segurança (sem recomendações financeiras)

---

## 👥 Público-Alvo

* Investidores iniciantes
* Idosos
* Pessoas com deficiência visual
* Pessoas com deficiência auditiva
* Pessoas neurodivergentes

---

## 🧠 Funcionalidades

### 💬 Chat Educacional com IA

* Integração com RAG
* Respostas contextualizadas
* Adaptação automática de linguagem

---

### 🧠 Quiz Interativo

* Perguntas com feedback inteligente
* Explicação gerada por IA
* Sistema de pontuação

---

### 🎮 Jogo Evolutivo

* Tomada de decisão financeira
* Progressão por fases
* Sistema de níveis e conquistas

---

### 🔊 Acessibilidade

* Áudio automático para deficiência visual
* Linguagem simplificada para idosos
* Estrutura lógica para neurodivergentes
* Texto claro para auditivos

---

## 🏗️ Arquitetura do Sistema

```
Usuário
   ↓
Streamlit (app.py)
   ↓
Lógica da BIA
   ├── Classificação de pergunta
   ├── Validação de segurança
   ├── Adaptação por público
   ↓
Contexto
   ├── Base interna (glossário)
   ├── RAG (FAISS + embeddings)
   ↓
LLM Local (Ollama)
   ↓
Pós-processamento
   ↓
Resposta final + Áudio (opcional)
```

---

## 🧠 Como a IA Funciona

### 🔎 RAG (Retrieval-Augmented Generation)

```
Pergunta do usuário
        ↓
Busca em documentos (data/)
        ↓
Geração de contexto
        ↓
LLM (Ollama)
        ↓
Resposta educativa
```

---

## 🔐 Segurança e Ética

* ❌ Não recomenda investimentos
* ❌ Não realiza previsões financeiras
* ❌ Não coleta dados do usuário
* ✅ Base de conhecimento controlada
* ✅ Respostas educativas e seguras

---

## 📁 Estrutura do Projeto

```
bia-academy-finance/
│
├── assets/        # Diagramas, mockups e imagens
├── data/          # Base de conhecimento (JSON, TXT)
├── docs/          # Demo (GitHub Pages)
│
├── src/
│   ├── app.py     # Interface + lógica principal
│   ├── meu_rag.py # Sistema de busca semântica
│
├── requirements/
│   └── requirements.txt
│
└── README.md
```

---

## 🧩 Stack Tecnológica

| Tecnologia            | Função                |
| --------------------- | --------------------- |
| Python                | Base da aplicação     |
| Streamlit             | Interface             |
| Ollama                | Execução de LLM local |
| Sentence Transformers | Embeddings            |
| FAISS                 | Busca vetorial        |
| gTTS                  | Geração de áudio      |
| NumPy                 | Processamento         |

---

## ⚙️ Como Executar

```bash
# Clonar repositório
git clone https://github.com/BARBARANFS/bia-academy-finance.git

cd bia-academy-finance

# Instalar dependências
pip install -r requirements/requirements.txt

# Iniciar IA local
ollama serve

# Rodar aplicação
streamlit run src/app.py
```

---

## 📊 Diferenciais do Projeto

* IA 100% local (sem custo)
* RAG aplicado na prática
* Inclusão digital real
* Experiência gamificada
* Arquitetura modular simples e funcional

---

## 🚀 Roadmap

### ✔ Concluído

* Chat com RAG
* Quiz com explicação inteligente
* Jogo evolutivo
* Áudio integrado

### 🔜 Evolução futura

* API da BIA
* Interface mobile
* Assistente por voz completo
* Integração com dados reais

---

## 👩‍💻 Autora

**Barbara Freitas**

🎓 Bootcamp Bradesco — GenAI & Dados
🤖 Foco em IA aplicada, educação e inclusão

---

## 📜 Licença

MIT License

---

## 💬 Mensagem Final

> Educação financeira não deve ser um privilégio.
> Deve ser acessível, inclusiva e baseada em tecnologia responsável.

---
