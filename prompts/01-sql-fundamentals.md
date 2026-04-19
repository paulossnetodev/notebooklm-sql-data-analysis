# Caso 1: Fundamentos do SQL aplicados à Análise de Dados

## 🎯 Objetivo

Entender as diferenças entre DDL, DML, DCL e TCL aplicadas ao contexto de análise de dados

---

## 🧠 Prompt Inicial

Explique DDL, DML, DCL e TCL no SQL

---

## ⚠️ Problemas encontrados

* Resposta genérica e teórica
* Ausência de exemplos práticos
* Nenhum contexto aplicado à análise de dados
* Não auxilia na tomada de decisão

---

## 🔧 Prompt Refinado

Explique as diferenças entre DDL, DML, DCL e TCL no SQL com exemplos práticos aplicados à análise de dados.

Para cada categoria:

* mostre uma query real
* explique quando um Data Analyst usaria
* cite erros comuns no uso

---

## ⚠️ Problemas ainda encontrados

* A IA não forneceu queries reais completas
* Exemplos ficaram descritivos, mas não executáveis
* Falta de profundidade em cenários reais

---

## 🧠 Correção aplicada (manual)

Para tornar o conteúdo aplicável, foram adicionados exemplos reais:

### 🔹 DML (exemplo real)

```sql
SELECT job_title, AVG(salary) AS avg_salary
FROM jobs
GROUP BY job_title;
```

**Uso:** análise de salários por cargo

---

### 🔹 DDL (exemplo real)

```sql
CREATE TABLE jobs_cleaned AS
SELECT * FROM jobs WHERE salary IS NOT NULL;
```

**Uso:** preparação de dados para análise

---

## 🧠 Aprendizado

* IA pode explicar conceitos corretamente, mas não necessariamente fornecer exemplos executáveis
* Prompts precisam exigir explicitamente código funcional
* Nem toda resposta da IA está pronta para uso real

---

## 🔍 Diagnóstico

O problema não foi apenas o prompt inicial, mas também a necessidade de validação crítica da resposta.

A IA respondeu corretamente em teoria, mas falhou em entregar profundidade prática.

---

## 🔁 Generalização do aprendizado

Para extrair valor real da IA:

* Sempre exigir exemplos executáveis
* Validar se a resposta pode ser aplicada em um banco real
* Complementar manualmente quando necessário

---
