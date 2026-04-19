<h1 align="center">💡 BIA Academy Finance</h1> 

<p align="center">
  <img src="https://raw.githubusercontent.com/BARBARANFS/bia-academy-finance/main/assets/imagens_readme/logo.png" width="200"/>
</p>

<p align="center">
  <b>Educadora Financeira Inclusiva com IA e Análise de Dados</b><br>
  <i>IA Generativa + Dados aplicados à educação financeira acessível, segura e personalizada</i>
</p>

---

## ♿ Acessibilidade como prioridade

Este projeto foi desenvolvido com foco em inclusão digital.

Atualmente, a **BIA Academy Finance** oferece **respostas em áudio automáticas para o público com deficiência visual**, permitindo acesso à educação financeira de forma mais acessível, clara e autônoma.

A solução foi projetada para evoluir continuamente, com o objetivo de expandir os recursos de acessibilidade para outros públicos, como idosos, pessoas com baixa alfabetização e usuários neurodivergentes.

🎧 Teste a demonstração:  
https://BARBARANFS.github.io/bia-academy-finance/

---

<p align="center">

![Python](https://img.shields.io/badge/Python-3.10%2B-blue?style=for-the-badge\&logo=python)
![Streamlit](https://img.shields.io/badge/Streamlit-App-red?style=for-the-badge\&logo=streamlit)
![AI](https://img.shields.io/badge/AI-Local-green?style=for-the-badge)
![RAG](https://img.shields.io/badge/RAG-Enabled-purple?style=for-the-badge)
![Data](https://img.shields.io/badge/Data-Driven-orange?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Concluído-success?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-lightgrey?style=for-the-badge)

</p>

---

## 🎯 Contexto

Projeto desenvolvido no **Bootcamp Bradesco — GenAI & Análise de Dados (DIO)**, com foco na aplicação prática de:

* IA Generativa
* RAG (Retrieval-Augmented Generation)
* Análise e estruturação de dados
* Experiência inclusiva

O projeto demonstra como **dados + IA** podem ser utilizados para construir soluções com impacto real.

---

## 📌 Visão Geral

A **BIA Academy Finance** é uma aplicação que atua como uma **educadora financeira digital**, integrando:

* 💬 Chat com IA
* 🧠 Quiz interativo
* 🎮 Jogo educacional
* 📊 Camada de dados estruturados
* 🔊 Acessibilidade
* 🔐 Segurança educacional

---

## ❌ Problema

A educação financeira ainda apresenta barreiras significativas:

* Linguagem técnica complexa
* Falta de acessibilidade
* Baixa personalização
* Exclusão de diferentes perfis de usuários

---

## ✅ Solução

A BIA resolve esses problemas através de:

* IA **100% local (offline)**
* Sistema **RAG baseado em dados estruturados**
* Adaptação por perfil de usuário
* Experiência interativa e gamificada
* Foco em **educação (não recomendação financeira)**

---

## 👥 Público-Alvo

* Investidores iniciantes
* Idosos
* Pessoas com deficiência visual
* Pessoas com deficiência auditiva
* Pessoas neurodivergentes

---

## 🧠 Funcionalidades

### 💬 Chat com IA

* Respostas contextualizadas via RAG
* Interpretação de intenção
* Adaptação automática de linguagem

---

### 🧠 Quiz

* Feedback educativo
* Explicação gerada por IA
* Sistema de pontuação

---

### 🎮 Jogo

* Simulação de decisões financeiras
* Progressão por fases
* Níveis e conquistas

---

### 🔊 Acessibilidade

* Áudio automático para deficiência visual  
* Linguagem simplificada e adaptativa  
* Estrutura personalizada por perfil de usuário  
* Base preparada para expansão de acessibilidade  

---

## 🏗️ Arquitetura do Sistema

```

Usuário
↓
Streamlit (app.py)
↓
Lógica da BIA
├── Classificação
├── Segurança
├── Adaptação
↓
Camada de Dados
├── Base interna (glossário)
├── RAG (FAISS + embeddings)
↓
LLM Local (Ollama)
↓
Resposta + Áudio

```

---

## 📊 Camada de Dados e Análise

A BIA Academy Finance aplica conceitos de **análise de dados** integrados à IA generativa.

### 🔍 Uso de dados no sistema

* Estruturação da base (`data/`)
* Organização de conteúdos educacionais
* Recuperação contextual (RAG)
* Interpretação de intenção do usuário

---

### 📈 Dados como suporte à decisão

Os dados permitem:

* Melhorar precisão das respostas
* Garantir aderência ao escopo educacional
* Adaptar linguagem por perfil
* Monitorar qualidade e performance

---

### 🧠 Integração Dados + IA

```

Dados → Contexto → IA → Resposta educativa

```

📌 Representa o ciclo:

**Dados → Informação → Inteligência → Decisão**

---

## 📊 Métricas, Dados e Observabilidade

As métricas são baseadas no comportamento real da aplicação.

### ✔ Qualidade Educacional

* Explicações claras e estruturadas
* Taxa estimada de acerto: **> 95%**

---

### 🔒 Segurança

* Bloqueio total de recomendações financeiras
* 100% aderente ao escopo educacional

---

### 🌍 Inclusividade

* Adaptação por público funcional
* Destaque: iniciantes, idosos e acessibilidade

---

### ⚡ Performance

* RAG: ~0.07s
* IA: ~120s (**principal gargalo**)

📌 Meta futura: < 5s

---

### 🧪 Robustez

* Interpretação de inputs informais
* Tratamento correto de:

  * Fora de escopo
  * Fallback
  * Restrições

---

## 📁 Estrutura do Projeto

```

bia-academy-finance/
│
├── assets/
├── data/
├── docs/
├── src/
│   ├── app.py
│   ├── meu_rag.py
│
├── requirements/
└── README.md

````

---

## 🧩 Stack Tecnológica

| Tecnologia            | Função         |
| --------------------- | -------------- |
| Python                | Backend        |
| Streamlit             | Interface      |
| Ollama                | LLM local      |
| Sentence Transformers | Embeddings     |
| FAISS                 | Busca vetorial |
| gTTS                  | Áudio          |

---

## ⚙️ Como Executar

```bash
git clone https://github.com/BARBARANFS/bia-academy-finance.git

cd bia-academy-finance

pip install -r requirements/requirements.txt

ollama serve

streamlit run src/app.py
````

---

## 🚀 Roadmap

### ✔ Concluído

* Chat com RAG
* Quiz inteligente
* Jogo educacional
* Áudio integrado (deficiência visual)

---

### 🔜 Próximos passos

* API da BIA
* Interface mobile
* Assistente por voz completo (entrada e saída)
* Expansão da acessibilidade para outros públicos
* Redução de latência

---

## 📈 Impacto

* Democratiza a educação financeira
* Reduz barreiras cognitivas
* Promove inclusão com tecnologia
* Aplica dados + IA em contexto real

### ♿ Inclusão como pilar

A acessibilidade na BIA não é um recurso isolado, mas um princípio de design.

O projeto inicia com suporte a deficiência visual e evolui com foco em ampliar o acesso à educação financeira para diferentes perfis de usuários.

---

## 🌍 Por que este projeto importa?

A exclusão financeira não é apenas econômica — é também educacional.

Milhões de pessoas não investem ou não organizam suas finanças por falta de acesso a conteúdos claros e acessíveis.

A BIA Academy Finance utiliza Inteligência Artificial para reduzir essa barreira, oferecendo:

* 📚 Educação financeira simplificada
* 🧠 Explicações adaptadas ao público
* ♿ Recursos de acessibilidade por voz

Este projeto busca democratizar o acesso ao conhecimento financeiro de forma inclusiva, ética e responsável.

---

## 👩‍💻 Autora

**Barbara Freitas**

🎓 Bootcamp Bradesco — GenAI & Dados
🤖 IA aplicada, análise de dados e inclusão

🔗 GitHub: [https://github.com/BARBARANFS](https://github.com/BARBARANFS)
🔗 LinkedIn: [https://www.linkedin.com/in/barbaranfreitas-accounting](https://www.linkedin.com/in/barbaranfreitas-accounting)

---

## 📜 Licença

MIT License

---

## 💬 Mensagem Final

> Educação financeira não deve ser privilégio.
> Deve ser acessível, inclusiva e construída com dados e inteligência artificial.

```

