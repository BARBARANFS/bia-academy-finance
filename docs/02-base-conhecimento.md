# 📚 Base de Conhecimento — BIA Academy Finance

## 🎯 Visão Geral

A base de conhecimento da **BIA Academy Finance** sustenta todas as respostas educacionais do sistema, garantindo clareza, confiabilidade e acessibilidade.

A arquitetura foi projetada para oferecer explicações financeiras de forma **simples, segura e adaptada ao perfil do usuário**, utilizando inteligência artificial e dados estruturados.

---

## 🗂️ Dados Utilizados

Os dados são armazenados localmente na pasta `data` e organizados da seguinte forma:

| Arquivo                         | Formato  | Utilização                            |
| ------------------------------- | -------- | ------------------------------------- |
| `MINIGUIA_SFN_INVESTIMENTOS.md` | Markdown | Base conceitual principal             |
| `GLOSSÁRIO DE CONCEITOS.md`     | Markdown | Simplificação de termos técnicos      |
| `Quizzes_investimentos.json`    | JSON     | Perguntas educativas com feedback     |
| `Jogos_inclusivos.json`         | JSON     | Narrativas interativas e aprendizagem |

---

## 🧠 Arquitetura

A BIA utiliza uma arquitetura híbrida composta por três componentes principais:

* **Biblioteca interna** → respostas rápidas e fallback
* **RAG (busca semântica)** → recuperação de conteúdo relevante
* **LLM (Ollama)** → geração da resposta final

Esses componentes trabalham juntos para gerar respostas **contextualizadas, didáticas e seguras**.

---

## 🔄 Fluxo da Resposta

1. Usuário envia a pergunta
2. Identificação do perfil do usuário
3. Consulta na biblioteca interna
4. Busca de contexto via RAG
5. Combinação das informações
6. Geração da resposta pelo modelo de IA
7. Adaptação da linguagem ao perfil
8. Retorno da resposta

---

## 🧪 Módulos do Sistema

### 💬 Chat

* Respostas dinâmicas com RAG + IA
* Explicações adaptadas ao usuário

### 🧠 Quiz

* Baseado em `Quizzes_investimentos.json`
* Feedback educativo com apoio da IA

### 🎮 Jogo

* Baseado em `Jogos_inclusivos.json`
* Aprendizado por decisões e progressão

---

## 🎯 Personalização

A BIA adapta automaticamente as respostas conforme o perfil do usuário:

* Investidor iniciante
* Idosos
* Deficiência visual (com áudio)
* Deficiência auditiva
* Neurodivergentes

A adaptação ocorre por meio de:

* Linguagem
* Estrutura da explicação
* Exemplos utilizados

---

## 🔒 Limitações

A BIA Academy Finance é uma ferramenta educacional e possui restrições:

* Não recomenda investimentos
* Não faz previsões de mercado
* Não analisa ativos específicos

### 🚫 Casos Bloqueados

| Tipo de Pergunta     | Comportamento               |
| -------------------- | --------------------------- |
| Recomendação         | Resposta bloqueada          |
| Fora do escopo       | Redirecionamento            |
| Produto desconhecido | Sugestão de fontes externas |

---

## 🧩 Inclusão

O sistema foi projetado para ser inclusivo, garantindo acesso ao aprendizado financeiro para diferentes perfis, com foco em:

* Clareza
* Acessibilidade
* Didática

---

## 📌 Conclusão

A base de conhecimento da **BIA Academy Finance** foi projetada como um sistema:

* Simples
* Eficiente
* Seguro
* Inclusivo

Garantindo educação financeira acessível e adaptada a diferentes públicos.
