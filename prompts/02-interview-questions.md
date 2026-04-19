# Caso: Geração de Perguntas de SQL

## 🎯 Objetivo

Gerar perguntas relevantes de SQL para preparação de entrevistas de Data Analyst

---

## 🧠 Prompt Inicial

Me dê perguntas de SQL

---

## ⚠️ Problemas encontrados

* A resposta inicial não considerava contexto de entrevistas reais
* Faltava profundidade técnica nas perguntas
* Ausência de exemplos práticos com queries

---

## 🔧 Prompt Refinado

Simule uma entrevista para Data Analyst com perguntas de SQL envolvendo JOIN, GROUP BY e agregações, incluindo respostas comentadas

---

## ✅ Resultado

A resposta passou a incluir:

* Estrutura de entrevista real
* Perguntas contextualizadas
* Explicações detalhadas
* Aplicação prática (ex: anti-join, agregações, lógica de execução)

Exemplo gerado:

```sql
SELECT date, SUM(amount) AS total_diario
FROM transactions
GROUP BY date
ORDER BY date DESC;
```

**Análise:**

* Uso correto de agregação com `SUM()`
* Aplicação adequada de `GROUP BY`
* Ordenação para análise temporal
* Query simples, mas alinhada com cenário real de negócio

---

## 📚 Referência das respostas

Baseado nas fontes carregadas no NotebookLM:
- Vídeos de SQL (YouTube)
- Artigo do Dataquest sobre entrevistas SQL

---

## 🧠 Aprendizado

* Prompts genéricos geram conteúdo superficial
* Adicionar contexto ("entrevista", "Data Analyst") melhora drasticamente a qualidade
* Pedir explicações comentadas aumenta o valor da resposta

---

## 🔍 Diagnóstico

O problema não estava apenas na IA, mas na falta de especificidade do prompt.

Sempre que quiser respostas mais profundas:

* Adicione contexto profissional
* Especifique técnicas (ex: JOIN, GROUP BY, etc.)
* Peça explicação + aplicação

---

## 🧠 Solução aplicada

* Adicionei contexto profissional ("Data Analyst")
* Especifiquei os tópicos técnicos (JOIN, GROUP BY, agregações)
* Solicitei respostas comentadas

---

## 📈 Resultado da melhoria

A qualidade da resposta aumentou em:

* Relevância para entrevistas reais
* Profundidade técnica
* Clareza na explicação

---

## 🔁 Generalização do aprendizado

O padrão utilizado neste caso pode ser aplicado em diversos contextos:

* Preparação para entrevistas técnicas
* Estudo guiado de conceitos complexos
* Simulação de cenários reais de análise de dados

A principal estratégia é transformar prompts genéricos em instruções específicas, com contexto, objetivo e restrições bem definidos.

---
