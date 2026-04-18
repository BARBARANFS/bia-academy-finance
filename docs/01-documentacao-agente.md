# 🤖 Documentação do Agente — BIA Academy Finance

## 🎯 Objetivo

A **BIA Academy Finance** é um agente de IA educacional focado em **educação financeira**, projetado para:

- Ensinar conceitos de investimentos de forma clara
- Adaptar a linguagem conforme o perfil do usuário
- Garantir segurança (sem recomendações financeiras)
- Operar com base em contexto real (RAG)

O sistema combina:

> **Interface (Streamlit) + IA local (Ollama) + Base de conhecimento (RAG) + Regras de negócio**

---

# 🧠 1. Funcionamento do Agente

## 🔄 Fluxo de execução

### Etapas:

1. Usuário envia pergunta
2. Sistema classifica o tipo de pergunta
3. RAG busca contexto relevante
4. IA gera resposta base
5. Resposta é adaptada ao público
6. Resposta final é exibida + áudio

---

# 🧩 2. Arquitetura do Sistema

## 📦 Componentes

| Camada | Tecnologia | Função |
|--------|-----------|--------|
| Interface | Streamlit | Interação com usuário |
| IA | Ollama (LLM local) | Geração de respostas |
| Base | Markdown + JSON | Conteúdo educacional |
| RAG | Indexação semântica | Recuperação de contexto |
| Regras | Python (app.py) | Controle de comportamento |

---

# 🧠 3. Classificação de Perguntas

A BIA classifica automaticamente a intenção do usuário:

| Tipo | Comportamento |
|------|-------------|
| Educacional | Explica conceitos financeiros |
| Restritiva | Bloqueia recomendações |
| Fora de escopo | Redireciona |
| Fallback | Responde ausência de informação |

---

## 📌 Exemplos reais

### ✔ Educacional
**Pergunta:**
> O que é liquidez?

**Resposta:**
Explica conceito + exemplo + aplicação

---

### 🔒 Restritiva
**Pergunta:**
> Qual investimento devo escolher?

**Resposta:**
> Posso te ajudar a entender, mas não posso recomendar um investimento específico.

---

### 🚫 Fora de escopo
**Pergunta:**
> Qual a previsão do tempo?

**Resposta:**
> Só posso responder sobre investimentos e educação financeira.

---

### ⚠️ Fallback
**Pergunta:**
> Quanto rende o produto XYZ?

**Resposta:**
> Não encontrei esse produto. Recomendo verificar na CVM ou B3.

---

# 🎯 4. Regras de Negócio (Core do Agente)

## 🔐 Segurança

A BIA:

- ❌ NÃO recomenda investimentos
- ❌ NÃO sugere ativos específicos
- ❌ NÃO faz previsões de mercado

---

## ✅ O que ela faz

- ✔ Explica conceitos financeiros
- ✔ Ensina boas práticas
- ✔ Usa exemplos do dia a dia
- ✔ Orienta sem induzir decisão

---

# 🌍 5. Adaptação por Público (Inclusividade Real)

A BIA adapta a resposta conforme o público selecionado no sistema.

---

## 👶 Investidor Iniciante

**Características:**
- Explicação progressiva
- Conceito → exemplo → impacto

**Exemplo:**
> Inflação é o aumento dos preços ao longo do tempo...

---

## 👴 Idoso

**Características:**
- Linguagem simples
- Tom acolhedor
- Exemplos cotidianos

**Exemplo:**
> A reserva de emergência é como uma proteção para imprevistos...

---

## 🧠 Neurodivergente

**Características reais:**
- Estrutura em blocos
- Explicação sequencial
- Reforço leve do conceito

**Observação:**
Ainda pode melhorar em:
- Redução de parágrafos longos

---

## 👂 Deficiência Auditiva

**Características:**
- Comunicação 100% textual
- Clareza direta
- Sem dependência de áudio

---

## 👁️ Deficiência Visual

**Características:**
- Compatível com leitura em voz
- Estrutura linear
- Conteúdo completo

---

# 🎧 6. Geração de Áudio

A BIA gera automaticamente áudio das respostas.

## Objetivo:
- Acessibilidade
- Inclusão (principalmente deficiência visual)
- Melhor experiência do usuário

---

# ⚙️ 7. Base de Conhecimento (RAG)

## 📚 Estrutura

A base contém:

- Conceitos financeiros
- Explicações estruturadas
- Exemplos práticos

---

## 🔎 Funcionamento

1. Pergunta do usuário é processada
2. Sistema busca conteúdo relevante
3. IA responde com base nesse contexto

---

## ✔ Benefícios

- Evita alucinação
- Garante consistência
- Usa conteúdo validado

---

# ⚠️ 8. Tratamento de Entrada do Usuário

A BIA é robusta para entradas imperfeitas.

## Exemplo real:

**Entrada:**
> oq hein inflação??

**Comportamento:**
- Interpreta corretamente
- Normaliza intenção
- Responde normalmente

---

# ⚡ 9. Performance do Sistema

## 📊 Estado atual

| Métrica | Valor |
|--------|------|
| Tempo RAG | ~0.07s |
| Tempo IA | ~120s |
| Tempo total | ~120s |

---

## 📉 Diagnóstico

- ✔ RAG eficiente
- ⚠ IA é gargalo principal

---

## 🎯 Meta ideal

| Métrica | Objetivo |
|--------|---------|
| Tempo total | < 5s |
| Tempo IA | < 3s |

---

# 📊 10. Observabilidade

## 🔍 Logs recomendados

- Pergunta do usuário
- Tipo de resposta
- Tempo de resposta
- Público selecionado

---

## 📈 KPIs

| KPI | Objetivo |
|-----|--------|
| Precisão | > 95% |
| Tempo médio | < 5s |
| Respostas fora de escopo | < 5% |
| Falhas de RAG | < 2% |

---

## 🚨 Alertas

- Tempo > 30s
- Falha de resposta
- Resposta fora do padrão

---

# 🧪 11. Casos de Teste Reais

✔ Educacional  
✔ Restrição  
✔ Fora de escopo  
✔ Fallback  
✔ Inclusividade por público  

---

# 🧩 12. Limitações Atuais

- Tempo de resposta elevado (IA local)
- Neurodivergente ainda pode melhorar estrutura
- Dependência de qualidade da base RAG

---

# 🚀 13. Roadmap de Evolução

- Redução de latência
- Melhor estrutura para acessibilidade cognitiva
- Expansão da base de conhecimento
- Monitoramento em tempo real

---

# 📌 Conclusão

A **BIA Academy Finance** é um agente de IA educacional com:

- Arquitetura sólida (RAG + IA local)
- Forte controle de segurança
- Alta qualidade educacional
- Inclusividade real por público

---
