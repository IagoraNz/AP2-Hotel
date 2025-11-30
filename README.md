# 🏨 AP2-Hotel: Sistema de Gerenciamento Hoteleiro

![Status do Projeto](https://img.shields.io/badge/Status-Concluído-green)
![C](https://img.shields.io/badge/C-10.3.0-blue)
![License](https://img.shields.io/badge/License-MIT-yellow)
![Nota Final](https://img.shields.io/badge/Nota%20Final-10%2F10-brightgreen)

Este repositório contém o trabalho final da 3ª avaliação da disciplina de **Algoritmos e Programação II**, ministrada pelo Professor Alan Rafael Ferreira dos Santos na Universidade Federal do Piauí - Campus Senador Helvídio Nunes de Barros, no curso de Bacharelado em Sistemas de Informação.

## 📄 Sobre o projeto

O objetivo deste projeto é criar um sistema de gerenciamento para um pequeno hotel. O sistema foi implementado em linguagem C e atende aos requisitos essenciais estabelecidos, proporcionando controle eficiente de reservas, clientes e pagamentos.

### 🎯 Objetivos específicos
- Gerenciar quartos do hotel (consulta, edição e exclusão).
- Controlar cadastro de clientes (registro, consulta, edição e exclusão).
- Gerenciar operações financeiras:
    - Realizar reservas
    - Efetuar check-in
    - Processar pagamentos
    - Consultar valores recebidos
- Implementar sistema de autenticação de funcionários.

## 🏗️ Estrutura do sistema

O sistema é organizado em módulos funcionais que gerenciam diferentes aspectos da operação hoteleira:

### Módulos principais
- **Quartos**: Gerenciamento completo de quartos (disponibilidade, edição, exclusão)
- **Clientes**: Controle de cadastro e informações de clientes
- **Reservas**: Sistema de reservas com verificação de disponibilidade
- **Financeiro**: Controle de pagamentos e relatórios financeiros
- **Funcionários**: Sistema de autenticação e cadastro de funcionários

## 🛠️ Tecnologias utilizadas

O projeto foi desenvolvido em **C** utilizando as seguintes ferramentas:

- **GCC**: Compilador GCC (tdm64-1) 10.3.0
- **Visual Studio Code**: Editor de código versão 1.89.1
- **Sistema de arquivos**: Persistência de dados em arquivos de texto

## 🚀 Como executar

### Pré-requisitos
Certifique-se de ter o GCC instalado em seu sistema.

### Compilação e execução

1. Clone o repositório:
   ```bash
   git clone https://github.com/IagoraNz/AP2-Hotel.git
   cd AP2-Hotel
   ```

2. Compile o projeto:
   ```bash
   gcc main.c -o hotel
   ```

3. Execute o programa:
   ```bash
   ./hotel
   ```

## 📋 Funcionalidades implementadas

### 🛏️ Gerenciamento de quartos
- **Consultar quarto**: Visualizar informações de quartos específicos
- **Editar quarto**: Modificar dados de quartos existentes
- **Excluir quarto**: Remover quartos do sistema

### 👥 Controle de clientes
- **Cadastrar cliente**: Registrar novos clientes no sistema
- **Consultar cliente**: Buscar informações de clientes
- **Editar cliente**: Atualizar dados de clientes
- **Excluir cliente**: Remover clientes do sistema

### 💰 Gestão financeira
- **Fazer reserva**: Permite reservar quartos, verificando disponibilidade e registrando dados como nome do cliente, número do quarto, datas, status de pagamento e valor total da reserva
- **Ver reserva**: Permite listar reservas de um cliente específico usando código de reserva ou nome do cliente
- **Excluir reserva**: Permite deletar uma reserva já realizada
- **Realizar check-in**: Habilita o registro de dados adicionais nos arquivos de quarto e reserva, alterando o status do quarto para ocupado e registrando data e hora de chegada do cliente
- **Efetuar pagamento**: Exibe o valor a ser pago pelo cliente, atualizando o status do quarto e registrando o valor pago no arquivo de controle financeiro
- **Valores recebidos**: Permite consulta de todos os valores recebidos durante um intervalo de tempo definido pelo usuário

## 📂 Estrutura do repositório

```
📂 AP2-Hotel/
├── 📂 db/                    # Banco de dados (arquivos de texto)
├── 📂 files/                 # Código fonte organizado por módulos
│   ├── 📂 Cliente/          # Módulo de gerenciamento de clientes
│   ├── 📂 Funcionario/      # Módulo de funcionários
│   ├── 📂 Menus/            # Interface de menus do sistema
│   ├── 📂 Quartos/          # Módulo de gerenciamento de quartos
│   ├── 📂 Reserva/          # Módulo de reservas
│   ├── 📂 checks/           # Validações e verificações
│   ├── 📄 struct.c          # Implementação de estruturas
│   └── 📄 struct.h          # Definição de estruturas
├── 📂 output/               # Arquivos de saída
├── 📄 main.c                # Arquivo principal do programa
└── 📄 README.md             # Documentação do projeto
```

## 📝 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.
