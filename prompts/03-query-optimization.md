# Caso: Otimização de Queries SQL em Ambiente de Produção

## 🎯 Objetivo

Entender como otimizar queries SQL considerando performance em grandes volumes de dados

---

## 🧠 Prompt Inicial

Otimize essa query SQL:

```sql
SELECT *
FROM transactions
WHERE YEAR(order_date) = 2023;
```

---

## ⚠️ Problemas encontrados

* Uso de `SELECT *` (retorno desnecessário de colunas)
* Uso de função `YEAR()` na cláusula WHERE
* Possível impedimento de uso de índices
* Alto risco de Full Table Scan

---

## 🔧 Prompt Refinado

Analise e otimize a query considerando ambiente com milhões de registros, incluindo análise de performance e boas práticas

---

## ✅ Resposta da IA (resumo)

A IA identificou corretamente:

* Problema de SARGability (uso de função na coluna)
* Risco de Full Table Scan
* Impacto em tabelas particionadas
* Ineficiência do `SELECT *`

---

## 🧪 Query otimizada sugerida

```sql
SELECT transaction_id, amount, order_date
FROM transactions
WHERE order_date >= '2023-01-01'
  AND order_date <= '2023-12-31';
```

---

## 🧠 Análise técnica

* Permite uso de índices (index seek)
* Evita processamento linha a linha
* Reduz I/O e uso de memória
* Torna a query escalável

---

## ⚠️ Limitações da resposta da IA

Apesar da boa análise, a IA não abordou:

* Diferença entre `BETWEEN` vs `>= e <` (edge cases de data/hora)
* Possível uso de índices compostos
* Impacto de timezone em colunas datetime
* Estratégias de particionamento mais avançadas

---

## 📈 Aprendizado

* Queries aparentemente corretas podem ser altamente ineficientes
* Pequenas mudanças podem gerar grande impacto em performance
* A IA pode identificar problemas, mas não cobre todos os cenários
* Pensamento crítico é essencial para validar otimizações

---

## 🔁 Generalização do aprendizado

Esse padrão se aplica a diversos cenários:

* Evitar funções em colunas filtradas
* Utilizar filtros que aproveitam índices
* Reduzir volume de dados retornados
* Pensar sempre em escalabilidade

---
