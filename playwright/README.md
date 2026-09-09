# Playwright

Este projeto demonstra testes de navegador com [Playwright Test](https://playwright.dev/). Os testes acessam `https://playwright.dev/` e validam o título da página e o link **Get started**.

## Pré-requisitos

- Node.js instalado, preferencialmente a versão LTS.
- npm instalado junto com o Node.js.
- Acesso à internet para baixar as dependências e executar os testes contra o site utilizado.

## Instalação

Abra um terminal na pasta `playwright`:

```bash
cd playwright
npm install
```

Depois, instale os navegadores usados pela configuração do projeto:

```bash
npx playwright install
```

No Linux, caso sejam necessárias as dependências do sistema, use:

```bash
npx playwright install --with-deps
```

## Executar os testes

Para executar todos os testes em Chromium, Firefox e WebKit:

```bash
npx playwright test
```

Para executar apenas um navegador:

```bash
npx playwright test --project=chromium
npx playwright test --project=firefox
npx playwright test --project=webkit
```

Para executar com o navegador visível:

```bash
npx playwright test --headed
```

Para acompanhar a execução passo a passo no modo de depuração:

```bash
npx playwright test --debug
```

## Relatório

A configuração gera um relatório HTML. Depois de executar os testes, abra-o com:

```bash
npx playwright show-report
```

Os testes estão em `tests/example.spec.js` e podem ser executados individualmente com:

```bash
npx playwright test tests/example.spec.js
```
