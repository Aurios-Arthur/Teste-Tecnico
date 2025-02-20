# Teste para Desenvolvedor Júnior - Sistema de Controle para Estética Automotiva

## Instruções Gerais
Você deve desenvolver uma aplicação simples para gerenciar serviços em uma estética automotiva. A aplicação deve ter um backend em **Node.js** e um frontend em **React**. O objetivo é avaliar suas habilidades em criar uma aplicação funcional, seguindo boas práticas de desenvolvimento.

Você terá **5 dias** para concluir o teste. Ao final, envie um link para o repositório no GitHub com o código fonte e instruções claras de como rodar o projeto.

## Requisitos do Sistema

### 1. Cadastro de Veículos
Crie uma tela para cadastrar veículos com os seguintes campos:
- **Placa** (obrigatório, formato válido de placa).
- **Marca** (obrigatório).
- **Modelo** (obrigatório).
- **Cor** (obrigatório).
- **Ano** (obrigatório, número válido).
- **Nome do Proprietário** (obrigatório).

Armazene os dados em um banco de dados (pode ser um arquivo JSON ou SQLite).

### 2. Agendamento de Serviços
Crie uma tela para agendar serviços com os seguintes campos:
- **Veículo** (selecione a partir dos veículos cadastrados).
- **Tipo de Serviço** (ex: lavagem, polimento, limpeza interna).
- **Data e Hora** (obrigatório, formato válido).
- **Observações** (opcional).

Valide se o horário está disponível (não permita agendamentos duplicados no mesmo horário).

### 3. Listagem de Serviços Agendados
Crie uma tela para listar todos os serviços agendados.
- Adicione um filtro para listar serviços por data.
- Mostre os detalhes de cada serviço (veículo, tipo de serviço, data, horário e status).

### 4. Atualização de Status do Serviço
Adicione um botão para atualizar o status do serviço. Os status possíveis são:
- **Agendado**
- **Em andamento**
- **Concluído**

### 5. Interface Simples
Crie uma interface básica em React com HTML e CSS.
- A interface deve ser intuitiva e responsiva (funcionar bem em dispositivos móveis).

## Tecnologias a Serem Utilizadas
- **Backend**: Node.js com Express.
- **Frontend**: React (use componentes funcionais e hooks).
- **Banco de Dados**: Pode ser um arquivo JSON ou SQLite.
- **Estilização**: CSS puro ou uma biblioteca como Bootstrap.

## O que Será Avaliado

- **Funcionalidade**: O sistema deve funcionar conforme os requisitos.
- **Organização do Código**: Separação de responsabilidades (frontend, backend, banco de dados), legibilidade e boas práticas de código.
- **Lógica de Programação**: Como você resolve problemas e implementa funcionalidades.
- **Conhecimento Técnico**: Uso correto de Node.js, React, HTML e JavaScript.
- **Documentação**: Instruções claras de como rodar o projeto.

## Entrega Esperada
- Um repositório no GitHub com o código fonte.
- Um arquivo `README.md` com:
  - Instruções para rodar o projeto.
  - Breve explicação das decisões técnicas.
- O projeto deve rodar localmente sem erros.

## Exemplo de Tarefas para o Candidato

### Backend (Node.js)
Crie uma API com as seguintes rotas:
- **POST /veiculos**: Cadastrar um veículo.
- **GET /veiculos**: Listar todos os veículos.
- **POST /servicos**: Agendar um serviço.
- **GET /servicos**: Listar todos os serviços.
- **PUT /servicos/:id**: Atualizar o status de um serviço.

Use um arquivo JSON ou SQLite para armazenar os dados.

### Frontend (React)
- Crie uma tela para cadastrar veículos.
- Crie uma tela para agendar serviços.
- Crie uma tela para listar serviços agendados com filtro por data.
- Adicione um botão para atualizar o status do serviço.

### Estilização
- Use CSS puro ou uma biblioteca como Bootstrap para estilizar a interface.
- Certifique-se de que a interface seja responsiva.

## Dicas
- Comece pelo backend, criando a API e testando com ferramentas como Postman ou Insomnia.
- Depois, desenvolva o frontend e integre com a API.
- Use componentes reutilizáveis no React para organizar melhor o código.
- Teste todas as funcionalidades antes de enviar o projeto.

## Exemplo de Estrutura do Projeto
'''bash 
/backend
  - server.js (ou index.js)
  /routes
    - veiculos.js
    - servicos.js
  /data
    - veiculos.json (ou banco SQLite)
/frontend
  /src
    /components
      - VeiculoForm.js
      - ServicoForm.js
      - ServicoList.js
    - App.js
    - index.js
  - package.json
README.md
'''
## Critérios de Avaliação

| Critério                | Peso  |
|-------------------------|-------|
| Funcionalidade          | 40%   |
| Organização do Código   | 20%   |
| Lógica de Programação    | 20%   |
| Conhecimento Técnico    | 10%   |
| Documentação            | 10%   |
