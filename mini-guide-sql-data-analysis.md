# 📘 Miniguia de SQL para Análise de Dados

## 🎯 Objetivo

Este miniguia consolida os principais aprendizados sobre SQL aplicado à análise de dados, com foco em revisão rápida, aplicação prática e uso estratégico do NotebookLM.

---

# 🧾 Resumo Estruturado

## 🔹 DDL (Data Definition Language)

Responsável pela definição da estrutura do banco de dados.

**Principais comandos:**

* CREATE
* ALTER
* DROP

**Uso na prática:**

* Criação de tabelas para dados limpos
* Alteração de estrutura para análise

---

## 🔹 DML (Data Manipulation Language)

Manipulação e consulta de dados.

**Principais comandos:**

* SELECT
* INSERT
* UPDATE
* DELETE

**Uso na prática:**

* Extração de insights
* Análise de dados
* Agregações (SUM, AVG, COUNT)

---

## 🔹 DCL (Data Control Language)

Controle de permissões.

**Principais comandos:**

* GRANT
* REVOKE

**Uso na prática:**

* Controle de acesso a dados sensíveis

---

## 🔹 TCL (Transaction Control Language)

Gerenciamento de transações.

**Principais comandos:**

* COMMIT
* ROLLBACK

**Uso na prática:**

* Garantia de consistência em alterações

---

# 🧠 Conceitos Avançados

## 🔹 JOINs

Combinação de tabelas para análise.

* INNER JOIN → apenas correspondências
* LEFT JOIN → mantém dados da esquerda

---

## 🔹 GROUP BY e Agregações

Permitem resumir dados:

```sql
SELECT job_title, AVG(salary)
FROM jobs
GROUP BY job_title;
```

---

## 🔹 Otimização de Queries

Boas práticas:

* Evitar `SELECT *`
* Não usar funções em colunas filtradas
* Utilizar índices
* Filtrar corretamente datas

---

# 📖 Glossário

* **SARGable** → Query que permite uso de índices
* **Full Table Scan** → Leitura completa da tabela
* **Index Seek** → Busca eficiente usando índice
* **CTE** → Consulta temporária reutilizável
* **JOIN** → Combinação de tabelas
* **Cardinalidade** → Distribuição dos dados
* **Partition Pruning** → Ignorar partições irrelevantes

---

# 🔁 Prompts Reutilizáveis

## 🔹 Aprendizado de conceitos

"Explique [conceito SQL] com exemplos aplicados à análise de dados"

---

## 🔹 Preparação para entrevistas

"Simule uma entrevista para Data Analyst com perguntas de SQL e respostas comentadas"

---

## 🔹 Otimização

"Otimize essa query SQL explicando performance e boas práticas"

---

## 🔹 Validação crítica

"Analise essa query SQL e identifique possíveis problemas de performance e integridade de dados"

---

# 🧠 Conclusões Finais

Saber SQL não é apenas escrever queries, mas:

* Entender o impacto das decisões na performance
* Validar criticamente soluções
* Utilizar IA como ferramenta estratégica de aprendizado

---
