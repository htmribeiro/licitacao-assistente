# 💻 Opção 2 – Com código (Low-code / Customizado com IA)

Ideal se você quiser algo mais robusto, com interface própria e banco de dados.

## O que você vai precisar:

* Linguagem de programação: Python

* Bibliotecas: LangChain, PyMuPDF ou PDFPlumber (pra ler PDF), OpenAI API ou LlamaIndex

* Banco de dados (opcional): SQLite, PostgreSQL ou até planilhas

* Interface (opcional): Streamlit ou Flask (pra usar via navegador)

* Estrutura básica:
  * Upload do edital (PDF)
  * Parser de PDF: extrai o texto do edital

* Classificador e interpretador: divide o texto em partes como:
  * Objeto da licitação
  * Requisitos de participação
  * Prazo de entrega
  * Documentos exigidos
  * Critério de julgamento

* Geração de resumo estruturado

* Exportação em planilha ou visualização em tela

* Exemplo de prompt para análise:

  * python
  * Copiar
  * Editar
  * prompt =
  
  ```txt
    """
    Você é um especialista em licitações públicas no Brasil.
    Analise o texto a seguir de um edital e me diga:
    1. Qual é o objeto da licitação?
    2. Quem pode participar?
    3. Quais documentos são exigidos?
    4. Quais são os prazos?
    5. Qual o critério de julgamento (menor preço, técnica e preço, etc)?

    Texto do edital: {conteudo_extraido}
    """
  ```
  