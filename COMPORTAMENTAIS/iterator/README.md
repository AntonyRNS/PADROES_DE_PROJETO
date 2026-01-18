# Padrão comportamental Iterator

## O que é

Iterator é um padrão comportamental que tem como foco fornecer uma forma de acessar sequencialmente os elementos de uma coleção, sem expor sua estrutura interna.

## Funcionamento

"O padrão Iterator permite que você percorra elementos de uma coleção sem revelar sua representação subjacente."

Basicamente, o Iterator separa a lógica de percurso da coleção da própria coleção, permitindo diferentes formas de iteração sem alterar a estrutura dos dados.

## Componentes

![alt text](image.png)

### Iterator
Define a interface para acessar e percorrer os elementos da coleção, como avançar e verificar se há próximo elemento.

### ConcreteIterator
Implementa a interface Iterator e mantém o controle da posição atual na coleção.

### Aggregate
Define a interface para criar um iterador.

### ConcreteAggregate
Implementa a interface Aggregate e retorna uma instância de um iterador concreto.

### Client
Utiliza o iterador para percorrer os elementos da coleção, sem conhecer sua estrutura interna.

## Vantagens e desvantagens

### Vantagens

- Acessa coleções sem expor sua estrutura interna
- Permite múltiplos tipos de iteração
- Princípio da responsabilidade única
- Princípio aberto/fechado
- Simplificação de código

### Desvantagens

- Aumenta a quantidade de classes
- Pode tornar o código mais complexo
- Pode ser desnecessário para coleções simples

## Referências
[Refactoring Guru](https://refactoring.guru/pt-br/design-patterns/iterator)
