# Padrão estrutural adapter

## O que é

Adapter é um padrão estrutural que tem como foco resolver ou amenizar o problema entre diferentes interfaces imcompatíveis.

## Funcionamento

"Essa implementação usa o princípio de composição do objeto: o adaptador implementa a interface de um objeto e encobre o outro. Ele pode ser implementado em todas as linguagens de programação populares."

Basicamente, fazendo uso de uma interface funcionando como tradutor, o adapter facilita a comunicação entre duas outras interfaces que não falam a mesma "lingua".

## Componentes

### Client
Faz a utilização do sistema, é responsável por trabalhar com outra interface não sabendo que ocorre uma adaptação.

### Adaptee
Interface-alvo que deve ser adaptada, sua interface é imcompativel com o que o client espera.

### Target
Molde que o sistema já conhece e considera como sendo o esperado.

### Adapter
Sendo o foco do padrão, o adapter faz a implementação da interface-alvo e encapsula a classe adaptada


![UML adapter](/PADROES_DE_PROJETO/ESTRUTURAIS/adapter/umladapter.png)

## Vantagens e desvantagens

### Vantagens

- Reutilização código existente (aberto/fechado)
- Responsabildiade única
- Baixo acoplamento

### Desvantagens

- Aumenta a quantidade de classes no projeto
- Aumento na complexidade do código
- Descnecessário para sistemas e problemas simples


## Referências
[Refactoring Guru](https://refactoring.guru/pt-br/design-patterns/adapter)