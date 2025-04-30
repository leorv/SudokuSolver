# 🧩 Sudoku Solver com API Externa

Este projeto é uma aplicação web simples que permite resolver tabuleiros de Sudoku utilizando uma API externa para processar a solução.

## 🎯 Objetivo

O projeto foi criado com o objetivo de exercitar o consumo de APIs e a integração entre frontend (HTML, CSS e JavaScript) e backend (Node.js com Express). O usuário pode preencher os valores de um tabuleiro de Sudoku manualmente, e ao clicar em "Solve", a aplicação envia os dados para uma API externa que retorna a solução (caso exista).

## 🛠 Tecnologias Utilizadas

### Frontend:
- HTML5
- CSS3
- JavaScript
- Axios

### Backend:
- Node.js
- Express.js
- CORS
- Dotenv
- [RapidAPI - solve-sudoku](https://rapidapi.com)

## 🧩 Funcionalidades

- Interface visual com grade 9x9 para entrada dos valores.
- Destaque visual para blocos 3x3 alternados com `odd-section`.
- Botão para solicitar a resolução do Sudoku.
- Envio dos dados ao backend, que repassa para a API externa.
- Exibição da solução na interface, caso seja possível.

## 🚀 Como Executar Localmente

1. **Clone o repositório:**
   ```bash
   git clone https://github.com/leorv/SudokuSolver.git
   cd SudokuSolver
   ```
   
2. Configure a chave da API:
  Crie um arquivo .env na raiz do projeto e adicione:

```
RAPID_API_KEY=SUA_CHAVE_AQUI
```

3. Instale as dependências do backend:

```
npm install
```

4. Inicie o servidor Node.js:

```
node server.js
```

Abra o index.html em seu navegador (dê duplo clique ou use uma extensão como Live Server).

## 📦 Estrutura do Projeto

```
SudokuSolver/
├── app.js          # Lógica JS do frontend
├── index.html      # Estrutura HTML
├── style.css       # Estilo da aplicação
├── server.js       # Servidor Node.js para lidar com requisições
├── .env            # Chave da API (não versionado)
```

## 📌 Observações

É necessário ter uma conta na RapidAPI para gerar sua chave.

O backend precisa estar rodando para o frontend conseguir fazer a solicitação da solução.

O projeto é voltado para fins educacionais e de aprendizado em integração de sistemas.

Desenvolvido por Leonardo Ruoso Vendramini
