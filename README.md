# Sistema Bancário

Este documento apresenta a documentação técnica para o programa "Sistema Bancário", um sistema bancário básico com funcionalidades de depósito, saque e extrato.

## 1. Introdução

O programa "Sistema Bancário" foi desenvolvido com o objetivo de simular um sistema bancário básico, demonstrando as funcionalidades essenciais de um sistema financeiro.

## 2. Arquitetura

O programa é implementado em Python e possui uma estrutura simples, composta por:

- **Variáveis globais**: Armazenam os dados da conta, como saldo, limite, extrato, número de saques e limites de saques.
- **Função main**: Contém o loop principal do programa, responsável por apresentar o menu de opções ao usuário e gerenciar a interação com o sistema.
- **Funções auxiliares**: Realizam as operações de depósito, saque e extrato.

## 3. Funcionalidades

### 3.1 Depósito

- Permite adicionar valores ao saldo da conta.
- Valida se o valor informado é positivo.
- Atualiza o saldo e o extrato.

### 3.2 Saque

- Permite retirar valores do saldo da conta.
- Realiza as seguintes validações:
  - Verifica se o valor solicitado é menor ou igual ao saldo disponível.
  - Verifica se o valor solicitado é menor ou igual ao limite de saque.
  - Verifica se o número de saques permitidos ainda não foi atingido.
- Atualiza o saldo, o extrato e o número de saques realizados.

### 3.3 Extrato

- Apresenta o histórico de movimentações da conta.
- Exibe o saldo atual da conta.

### 3.4 Sair

- Encerra a execução do programa.

## Limitações

- O programa não possui autenticação de usuários, ou seja, qualquer pessoa pode utilizar o sistema.
- O limite de saques é fixo em 3 saques por sessão.
- O programa não salva os dados do usuário em arquivos, portanto, os dados são perdidos ao sair do programa.

## Como Utilizar

1. **Copie o código**: Copie o código Python apresentado no arquivo `banco_simples.py`.
2. **Execute o código**: Execute o código utilizando um interpretador Python.
3. **Interaja com o menu**: Utilize as opções numéricas do menu para realizar as operações desejadas.
