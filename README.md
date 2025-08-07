# 🧠 Atividade 2 – Perguntas e Respostas usando Modelos do Hugging Face

Este projeto realiza uma tarefa de **Perguntas e Respostas (Question Answering)** utilizando três modelos de linguagem disponibilizados pelo Hugging Face. As respostas são obtidas a partir da leitura de dois documentos: um PDF sobre **doenças respiratórias crônicas** e um DOCX contendo um **dicionário de dados**.

## 👤 Autor
- **Elison Monteiro Passos**

---

## 📄 Descrição da Atividade

A proposta da atividade é utilizar **modelos de NLP pré-treinados** para responder automaticamente perguntas com base em dois tipos de documentos. Foram utilizadas bibliotecas para extração de texto dos arquivos e os modelos foram avaliados de forma automática e manual.

---

## 📁 Documentos Utilizados

- `doencas_respiratorias_cronicas.pdf`: documento com informações médicas.
- `dicionario_de_dados.docx`: contém descrições de campos de bases de dados de saúde.

---

## ❓ Perguntas Utilizadas

### 📌 Documento: Doenças Respiratórias Crônicas

1. Quais são as atribuições do enfermeiro?  
2. O que é o aerosol e qual sua composição química?  
3. Quais são as doses recomendadas da substância Fenoterol de nome comercial Berotec para crianças?

### 📌 Documento: Dicionário de Dados

1. Qual a descrição do campo `PREFIXOMAQ` na tabela de perfil do gestor?  
2. Qual o tipo do campo `CNPJ_MANT` na tabela de estabelecimentos de saúde?  
3. Quais os domínios da coluna `NIVEL_DEP`, na tabela de estabelecimentos de saúde?

---

## 🤖 Modelos Utilizados

| Modelo | Arquitetura | Parâmetros | Link |
|--------|-------------|------------|------|
| `Falconsai/question_answering_v2` | DistilBERT | 66.4M | [Hugging Face](https://huggingface.co/Falconsai/question_answering_v2) |
| `usamakenway/Bert-question-answering-optimized` | BERT | - | [Hugging Face](https://huggingface.co/usamakenway/Bert-question-answering-optimized) |
| `deepset/xlm-roberta-large-squad2` | XLM-RoBERTa (Multilíngue) | 560M | [Hugging Face](https://huggingface.co/deepset/xlm-roberta-large-squad2) |

---

## 🛠️ Tecnologias e Bibliotecas

- `transformers`: para carregar e usar modelos de QA.
- `torch`: backend de deep learning.
- `pdfplumber`: extração de texto de PDF.
- `python-docx`: leitura de arquivos DOCX.
- `sklearn`: cálculo de métricas de avaliação (opcional).
- `matplotlib` ou `seaborn`: para visualizações gráficas (se aplicável).

---

## 🚀 Como Executar

1. Instale as dependências:
```bash
pip install transformers torch pdfplumber python-docx
