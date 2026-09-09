# Vitest

Este projeto demonstra testes unitários com [Vitest](https://vitest.dev/). O exemplo testa a função `sum`, localizada em `sum.js`, usando o arquivo `sum.test.js`.

## Pré-requisitos

- Node.js instalado, preferencialmente a versão LTS.
- npm instalado junto com o Node.js.

## Instalação

Abra um terminal na pasta `vitest`:

```bash
cd vitest
npm install
```

O comando instala o Vitest definido como dependência de desenvolvimento no `package.json`.

## Executar os testes

Para executar os testes uma vez, sem permanecer em modo de observação:

```bash
npx vitest run
```

Para executar o Vitest em modo de observação, repetindo os testes quando os arquivos forem alterados:

```bash
npm run test
```

Para executar somente o arquivo de teste do exemplo:

```bash
npx vitest run sum.test.js
```

Para gerar uma saída mais detalhada:

```bash
npx vitest run --reporter=verbose
```

O teste verifica se `sum(1, 2)` retorna `3`.
