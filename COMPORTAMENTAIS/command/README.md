# Padrão comportamental Command

## O que é

Command é um padrão comportamental que tem como foco encapsular uma solicitação como um objeto, permitindo parametrizar clientes com diferentes pedidos, enfileirar ou registrar comandos e suportar operações de desfazer (undo).

## Funcionamento

"O padrão Command transforma uma solicitação em um objeto independente que contém todas as informações sobre a solicitação."

Basicamente, a ação a ser executada é encapsulada em um objeto comando, separando quem solicita a ação de quem realmente a executa.

## Componentes

![alt text](image.png)

### Command
Define a interface comum para todos os comandos, geralmente com um método execute.

### ConcreteCommand
Implementa a interface Command e define a ligação entre a ação e o objeto que a executa.

### Receiver
É o objeto que realmente executa a ação solicitada pelo comando.

### Invoker
É responsável por disparar o comando, sem conhecer os detalhes da execução.

### Client
Cria e configura os comandos, associando-os aos receivers.

## Vantagens e desvantagens

### Vantagens

- Desacopla quem solicita a ação de quem a executa
- Permite implementar operações de desfazer (undo)
- Permite enfileirar e registrar comandos
- Princípio aberto/fechado
- Princípio da responsabilidade única

### Desvantagens

- Aumenta a quantidade de classes
- Pode tornar o código mais complexo
- Pode ser excessivo para ações simples

## Referências
[Refactoring Guru](https://refactoring.guru/pt-br/design-patterns/command)
