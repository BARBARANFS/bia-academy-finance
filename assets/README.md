# 📁 Assets — BIA Academy Finance

Esta pasta reúne os **recursos visuais, identidade visual e diagramas do sistema BIA Academy Finance**.

Ela é responsável por **documentar visualmente o projeto**, apoiar o README principal e reforçar a identidade da solução.

---

# 🎨 0. Identidade Visual (Logo)

A BIA Academy Finance possui uma identidade visual própria:


<p align="center">
  <img src="imagens_readme/logo.png" width="180"/>
</p>



### 📌 Uso do logo:

* README principal
* Apresentações (pitch)
* GitHub Pages
* Documentação

---

## 🧩 Estrutura da Pasta

assets/
├── diagramas/
│   └── arquitetura.md
├── screenshots/
│   ├── chat_tela.png
│   ├── quiz_tela.png
│   ├── jogo_tela.png
│   └── api_endpoint.png
├── mockups/
│   ├── quiz_mockup.md
│   └── jogo_mockup.md
└── imagens_readme/
    ├── fluxo.png
    └── inclusao.png



---

# 🧠 2. Arquitetura do Sistema (BIA REAL)

```
+---------+
| Usuário |
+---------+
     ↓
+---------------------------+
| app.py (Streamlit UI)     |
+---------------------------+
     ↓
+---------------------------+
| Lógica da Bia             |
| - Classificação           |
| - Segurança               |
| - Adaptação por público   |
+---------------------------+
     ↓
+----------------------+----------------------+
| Base local           | RAG (FAISS)          |
| (Glossário interno)  | Documentos externos  |
+----------------------+----------------------+
     ↓
+---------------------------+
| LLM Local (Ollama)        |
+---------------------------+
     ↓
+---------------------------+
| Resposta adaptada         |
+---------------------------+
     ↓
+---------------------------+
| Acessibilidade (Áudio)    |
+---------------------------+
```

---

# 🔄 3. Fluxo do Sistema

Usuário
↓
Interface (Streamlit)
↓
Escolha da funcionalidade

### 💬 Chat

Pergunta → RAG + Base interna → LLM → Resposta adaptada → (Áudio opcional)

### 🧠 Quiz

Pergunta → Resposta → Validação → Pontuação → Explicação com IA

### 🎮 Jogo

Fases → Decisão → Feedback → Pontuação → Nível → Conquistas

---

# 🎯 4. Conceitos-Chave

### ✔ Educação, não recomendação

A BIA ensina, mas não recomenda investimentos.

### ✔ Adaptação por público

* Iniciante
* Idoso
* Deficiência visual
* Deficiência auditiva
* Neurodivergente

### ✔ Segurança

* Bloqueio de recomendações
* Respostas controladas
* Base confiável

---

# 🧠 5. Mockup — Quiz

```
| BIA Academy Finance |

Pergunta: Qual investimento tem maior liquidez?

( ) Tesouro Selic
( ) LCI com carência
( ) Ações

[Responder]

💡 Feedback:
"O Tesouro Selic pode ser resgatado a qualquer momento."

🏆 +10 pontos
```

---

# 🎮 6. Mockup — Jogo

```
| BIA Academy Finance |

🧩 Fase 1
Você recebeu seu salário. O que fazer?

( ) Gastar tudo
( ) Guardar parte
( ) Ignorar planejamento

[Responder]

💡 "Guardar cria base financeira."

🏆 +20 pontos
```

---

# 🧠 7. Progressão

Pontuação:

* Quiz → +10
* Jogo → +20 / +30 / +50

Níveis:

* 0–49 → Iniciante
* 50–99 → Intermediário
* 100+ → Avançado

---

# 🎧 8. Acessibilidade

* 🔊 Áudio automático
* 🧠 Estrutura para neurodivergentes
* 👂 Texto claro
* 👵 Linguagem adaptada

---

# 📸 9. Screenshots

* chat_tela.png
* quiz_tela.png
* jogo_tela.png

---

# 🧭 10. Papel da Pasta Assets

A pasta **não contém código**, apenas:

* Documentação visual
* Apoio ao README
* Material para apresentação

---

# 🚀 11. Observação Final

A estrutura está **alinhada com o código real (`src/app.py`)**, garantindo:

* Coerência técnica
* Clareza para avaliadores
* Nível profissional (bootcamp + mercado)
