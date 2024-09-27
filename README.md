# Sistema de Gerenciamento Bancário

Este projeto é um sistema simples de gerenciamento bancário em Python, que permite criar clientes, contas bancárias e realizar transações como depósitos, saques e consulta de extratos.

## Funcionalidades

- **Clientes:** Cadastro de clientes com informações como CPF, nome, data de nascimento e endereço.
- **Contas Bancárias:** Criação de contas correntes para os clientes.
- **Transações:** Realização de depósitos, saques e consulta de extrato.
- **Histórico:** Cada conta possui um histórico de transações.

## Classes Principais

### 1. `Cliente`
Representa um cliente genérico que pode ter uma ou mais contas bancárias. Armazena o endereço do cliente e suas contas.

### 2. `PessoaFisica`
Herdeira de `Cliente`, representa um cliente pessoa física, com atributos adicionais como nome, CPF e data de nascimento.

### 3. `Conta`
Uma classe base que representa uma conta bancária com saldo, número da conta, agência e histórico de transações.

### 4. `ContaCorrente`
Herdeira de `Conta`, adiciona regras de limite de saque e quantidade máxima de saques por dia.

### 5. `Transacao`
Classe abstrata que define o comportamento básico de uma transação.

### 6. `Saque` e `Deposito`
Implementações da classe `Transacao` que representam, respectivamente, um saque e um depósito em conta.

### 7. `Historico`
Armazena e gerencia o histórico de transações realizadas em uma conta.

## Como usar

1. Clone este repositório.
2. Execute o script `main.py` para interagir com o sistema via terminal.
3. Use o menu para realizar as operações disponíveis: criar clientes, criar contas, depositar, sacar, consultar extratos, e listar contas.

### Exemplo de execução:

```bash
=============== MENU ================
[d]  Depositar
[s]  Sacar
[e]  Extrato
[nc] Nova conta
[lc] Listar contas
[nu] Novo usuário
[q]  Sair


Estrutura do Código

    Cliente e Contas: São criados para armazenar as informações dos clientes e contas bancárias.
    Transações: Depósitos e saques são implementados como classes específicas de transação.
    Histórico: Cada conta tem seu próprio histórico, registrando todas as transações realizadas.
    Menu: A interface do usuário é feita via linha de comando, oferecendo opções para gerenciar clientes e contas.

Tecnologias Utilizadas

    Python 3.10 ou superior
    Bibliotecas nativas: datetime, abc, textwrap

Executando o projeto

Certifique-se de ter o Python 3.x instalado em sua máquina. Para executar o projeto, siga os passos abaixo:

    Clone o repositório:


git clone https://github.com/seuusuario/seurepositorio.git

Navegue até o diretório do projeto:

cd seurepositorio

Execute o arquivo principal:


    python main.py

Contribuição

Se quiser contribuir com o projeto, sinta-se à vontade para fazer um fork e enviar um pull request. Sugestões, melhorias e correções são sempre bem-vindas!
Licença

Este projeto está sob a licença MIT. Consulte o arquivo LICENSE para mais detalhes.

Esse arquivo `README.md` dá uma visão geral do projeto, explica as funcionalidades pri
