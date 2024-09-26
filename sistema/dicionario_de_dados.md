# Dicionário de Dados:
- Descrição: Crie e mantenha um dicionário de dados que defina claramente todos os
dados utilizados no sistema.
- Conteúdo: Para cada dado, inclua:
    ▪ Nome do dado
    ▪ Tipo de dado (e.g., string, integer, date)
    ▪ Descrição (significado e uso do dado)
    ▪ Formato (como os dados são estruturados, e.g., yyyy-mm-dd para datas)
    ▪ Restrições (limitações ou validações aplicáveis, e.g., valores permitidos,
    comprimento máximo)
    ▪ Relacionamentos (como o dado se relaciona com outros dados no sistema)

##Entidades 
### Usuário

| Nome do Dado  |  Tipo de Dado |   Tamanho     |    Descrição   |   Restrição   |
| ------------- | ------------- | ------------- | ------------- | ------------- |
|     id        |    inteiro    |    4 bytes    | identificador único        | Chave principal, não pode ser vazio, auto incrementado |
| Primeiro nome |    varchar    |   30 bytes    | Primeiro nome do usuário   | Não pode ser vazio |
|  Último nome  |    varchar    |   30 bytes    | Último nome do usuário     | Não pode ser vazio |
|    email      |    varchar    |   60 bytes    | Endereço de email          | Não pode ser vazio |
|    senha      |    varchar    |   30 bytes    | Senha de 8-12 caracteres, com pelo menos uma letra maiúscula, minúscula ou símbolo. | Não pode ser vazio  |

### Professor
| Nome do Dado  |  Tipo de Dado |   Tamanho     |    Descrição   |   Restrição   |
| ------------- | ------------- | ------------- | ------------- | ------------- |
|     id        |    inteiro    |    4 bytes    | identificador único      | Chave principal, não pode ser vazio, auto incrementado |
|    siape      |    varchar    |    8 bytes    |                          | Não pode ser vazio |
| Primeiro nome |    varchar    |   30 bytes    | Primeiro nome do usuário | Não pode ser vazio |
|  Último nome  |    varchar    |   30 bytes    | Último nome do usuário   | Não pode ser vazio |

### Disciplina
| Nome do Dado  |  Tipo de Dado |   Tamanho     |    Descrição   |   Restrição   |
| ------------- | ------------- | ------------- | -------------  | ------------- |
|     id        |    inteiro    |    4 bytes    | identificador único   | Chave principal, não pode ser vazio, auto incrementado |
|    nome       |    varchar    |   30 bytes    | Nome da disciplina    | Não pode ser vazio |
|   código      |    varchar    |   10 bytes    | Código da disciplina  | Não pode ser vazio |

### Espaço Físico
| Nome do Dado  |  Tipo de Dado |   Tamanho     |    Descrição   |   Restrição   |
| ------------- | ------------- | ------------- | ------------- | ------------- |
|     id        |    inteiro    |    4 bytes    | identificador único| Chave principal, não pode ser vazio, auto incrementado |
|    floor      |    inteiro    |    4 bytes    |                                 | Não pode ser vazio |
|    numero     |    inteiro    |    4 bytes    |          | Não pode ser vazio |
|   situação    |    varchar    |    1 bytes    |  Situação do espaço, se está disponível ou sendo utilizado          | Não pode ser vazio |
|    tipo       |     bit       |    1 bytes    |  Tipo de espaço físico          | Não pode ser vazio |
