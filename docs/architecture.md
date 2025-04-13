# Arquitetura do Projeto

## Overview

O projeto segue uma arquitetura baseada em serviços composta por:

- **Frontend**: Interface gráfica para interação com o usuário.
- **Backend**: APIs REST para processamento dos editais.
- **Processamento**: Utiliza técnicas de NLP para interpretar o conteúdo.

## Fluxo de Dados
1. O usuário faz upload de um edital via Frontend.
2. O Backend processa o arquivo e utiliza NLP para interpretá-lo.
3. O resumo gerado é enviado de volta para o Frontend para exibição.

## Diagrama da Estrutura


```txt
licitacao-assistente/
├── backend/
│   ├── app/
│   │   ├── main.py
│   │   ├── models/
│   │   └── services/
│   ├── requirements.txt
│   └── tests/
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   └── App.js
│   ├── package.json
│   └── public/
├── docs/
│   ├── requirements.md
│   └── architecture.md
├── README.md
└── .gitignore
```
