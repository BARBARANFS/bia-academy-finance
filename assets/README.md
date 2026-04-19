# 📁 Assets — BIA Academy Finance

Esta pasta contém os recursos visuais, diagramas e representações do funcionamento do sistema BIA Academy Finance.

Seu objetivo é documentar de forma clara a arquitetura, o fluxo e a experiência do usuário, alinhados com a implementação real do projeto.

---

# 🧩 1. Estrutura da Pasta

assets/
├── diagramas/
│   └── arquitetura.md        # Arquitetura real do sistema
├── screenshots/
│   ├── chat_tela.png         # Tela do chat funcionando
│   ├── quiz_tela.png         # Tela do quiz
│   └── jogo_tela.png         # Tela do jogo evolutivo
├── mockups/
│   ├── quiz_mockup.md        # Representação simplificada do quiz
│   └── jogo_mockup.md        # Representação do jogo evolutivo
└── imagens_readme/
    ├── fluxo.png             # Fluxo geral do sistema
    └── inclusao.png          # Públicos atendidos

---

# 🧠 2. Arquitetura do Sistema (BIA REAL)

A arquitetura da BIA Academy Finance é local, modular e orientada à educação financeira inclusiva.

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

---

# 🔄 3. Fluxo de Funcionamento

O sistema é dividido em três módulos principais escolhidos diretamente pelo usuário:

Usuário
   ↓
Interface (Streamlit - app.py)
   ↓
Seleção de módulo

├── 💬 Chat Educacional
│   → Pergunta do usuário
│   → Classificação de intenção
│   → Busca de contexto (Glossário + RAG)
│   → Geração de resposta (LLM)
│   → Adaptação por público
│   → (Opcional) Geração de áudio
│
├── 🧠 Quiz Educativo
│   → Pergunta estruturada (JSON)
│   → Resposta do usuário
│   → Validação da resposta
│   → Pontuação (+10)
│   → Atualização de nível
│   → Explicação com IA + RAG
│
└── 🎮 Jogo Evolutivo
    → Sistema de fases progressivas
    → Escolha do usuário
    → Feedback imediato
    → Pontuação variável (20 / 30 / 50)
    → Progressão de nível
    → Sistema de conquistas
    → Ranking final

---

# 🎯 4. Conceitos-Chave do Sistema

## 🔹 Escolha do Usuário
O usuário decide qual experiência utilizar:
- Chat
- Quiz
- Jogo

## 🔹 Adaptação por Público
A Bia adapta a comunicação conforme o perfil selecionado:
- Investidor iniciante
- Idoso
- Deficiência auditiva
- Deficiência visual
- Neurodivergente

## 🔹 Educação, não recomendação
O sistema:
- Explica conceitos financeiros
- Usa exemplos práticos
- NÃO recomenda investimentos

## 🔹 Segurança
- Bloqueio de recomendações
- Respostas baseadas em contexto (RAG + base interna)
- Controle de linguagem

---

# 🧠 5. Mockup — Quiz

| BIA Academy Finance |

Pergunta: Qual investimento tem maior liquidez?

( ) Tesouro Selic  
( ) LCI com carência  
( ) Ações  

[Responder]

💡 Feedback:
"O Tesouro Selic pode ser resgatado a qualquer momento."

🏆 Pontuação: +10  
📊 Nível: atualizado automaticamente

---

# 🎮 6. Mockup — Jogo Evolutivo

| BIA Academy Finance |

🧩 Fase 1  
Você recebeu seu salário. O que fazer primeiro?

( ) Gastar tudo  
( ) Guardar parte  
( ) Ignorar planejamento  

[Responder]

💡 Feedback:
"Guardar cria base financeira."

🏆 Pontuação: +20  
📊 Nível: Iniciante → Intermediário  

---

# 🧠 7. Lógica de Progressão

## Pontuação
- Quiz: +10 por acerto
- Jogo: +20 / +30 / +50 por fase

## Níveis
- 0 a 49 → Iniciante  
- 50 a 99 → Intermediário  
- 100+ → Avançado  

## Conquistas
- 🎯 Primeira conquista → 20 pontos  
- 🏆 100 pontos → 100 pontos  
- 🚀 Jornada completa → finalizar fases  

## Ranking
- Top 5 jogadores
- Ordenado por pontuação

---

# 🎧 8. Acessibilidade

A BIA Academy Finance possui recursos de inclusão:

- 🔊 Áudio automático (para deficiência visual)
- 🧠 Respostas estruturadas (neurodivergentes)
- 👂 Texto simplificado (deficiência auditiva)
- 👵 Linguagem adaptada (idosos)

---

# 📸 9. Screenshots

As imagens desta pasta representam a interface real do sistema:

- chat_tela.png → Conversa com IA
- quiz_tela.png → Sistema de perguntas
- jogo_tela.png → Jornada evolutiva

---

# 🧭 10. Considerações Finais

A pasta `assets` não contém lógica de código.

Seu papel é:
- Documentar visualmente o sistema
- Facilitar entendimento do projeto
- Apoiar apresentações e validações

Toda a lógica funcional está na pasta `src/`.
