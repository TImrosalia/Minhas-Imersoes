# Aula 05 - Criando um sistema para busca em documentos usando Embeddings e a Gemini API

Nesta aula, criamos um sistema capaz de buscar informações em documentos utilizando a técnica de **embeddings** e a **API do Gemini**. A proposta foi explorar como fazer com que a IA entenda o conteúdo de textos e encontre respostas relevantes, mesmo que não sejam idênticas à pergunta feita.

## ✨ Conceitos abordados

- **Embeddings**: Transformam palavras, frases ou imagens em vetores numéricos (códigos) para que os computadores consigam interpretá-los.
- **Gemini API**: Ferramenta da Google que gera respostas com base em instruções e contexto (prompt).
- **Função apply**: Aplica uma função a cada elemento (linha ou coluna) de um DataFrame do Pandas.
- **Função lambda**: Define funções sem precisar dar nome.
- **Stack**: Pilha de instruções/respostas em sequência.
- **NLP (ou PLN)**: Processamento de Linguagem Natural — área da IA que trabalha com textos.
  
## 📚 Bibliotecas utilizadas

- `pandas`: manipulação de dados tabulares.
- `numpy`: operações matemáticas.
- `requests`: fazer requisições HTTP para consumir APIs.
- `matplotlib`: (opcionalmente usada) para gráficos e visualizações.
  
## 🧠 Objetivo do projeto

Desenvolver um buscador semântico, ou seja, um sistema que entende o **significado** da pergunta e retorna trechos relevantes dos documentos — mesmo que as palavras exatas não coincidam. Ideal para quem deseja criar sistemas de consulta inteligente em textos grandes (como FAQs, contratos, e-books etc).

## 📝 Observações

- Utilizamos um CSV de documentos e extraímos seus embeddings.
- A pergunta do usuário também é convertida em embedding.
- Calculamos a **semelhança vetorial** (normalmente via cosseno) entre a pergunta e os documentos.
- O trecho mais próximo é enviado para a **Gemini API**, que gera uma resposta contextualizada.
  
## 🧪 Arquivo da aula

> [`Sistema_de_busca_Embeddings_e_a_Gemini_API_aula05.ipynb`](./Sistema_de_busca_Embeddings_e_a_Gemini_API_aula05.ipynb)

---

📅 _Data da aula: 12/05/2024_

---

