# UsesCaseEntidProduct

Implementação do desafio **Clean Architecture: Use Cases para a Entidade Product** usando o template obrigatório:

https://github.com/devfullcycle/fc-clean-architecture.git

## Escopo Implementado

Foram criados os 4 Use Cases da entidade Product:

- CreateProductUseCase
- FindProductUseCase
- ListProductUseCase
- UpdateProductUseCase

Cada Use Case possui DTOs de entrada/saída e testes obrigatórios:

- Teste de unidade com mock do repository.
- Teste de integração com Sequelize e SQLite em memória.

## Instalação

```bash
npm install
```

No Windows, caso o PowerShell bloqueie o comando `npm`, use:

```bash
npm.cmd install
```

## Executar os Testes

```bash
npm run test
```

No Windows:

```bash
npm.cmd run test
```

O script executa:

```bash
npm run tsc -- --noEmit && jest
```

## Resultado Validado

Execução realizada com sucesso:

```text
Test Suites: 27 passed, 27 total
Tests:       67 passed, 67 total
Snapshots:   0 total
```

## Estrutura Principal

```text
src/usecase/product/
|-- create/
|-- find/
|-- list/
`-- update/
```

Cada pasta possui:

- DTO
- Use Case
- Teste unitário
- Teste de integração

