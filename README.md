# Projeto_Integrador_2
## Projeto Integrador 2 - Univesp
Criada a modelagem de dados para a aplicação Gestão Orcamentária

 ```mermaid
classDiagram
  class Cliente {
    - nome: String
    - logradouro: String
    - numero: String
    - email: String
    - cpf: String
    - cep: String
  }

  class Servico {
    - tipo: String
    - quantidade: Integer
    - preco: Integer
  }

  class Orcamento {
    - tipo_servico: String
    - preco_servico: Integer
  }

  Cliente "1" *-- "N" Servico
  Cliente "1" *-- "N" Orcamento
```

