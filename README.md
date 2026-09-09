# Ferramentas de Testes

Este repositório contém o trabalho da disciplina de **Validação e Verificação**, com exemplos de uso de duas ferramentas de testes para JavaScript:

- **Playwright**: testes automatizados de aplicações web em Chromium, Firefox e WebKit.
- **Vitest**: testes unitários rápidos para funções JavaScript.

## Pré-requisitos

- Node.js instalado, preferencialmente a versão LTS.
- npm, instalado junto com o Node.js.
- Acesso à internet para baixar as dependências e, no caso do Playwright, acessar a página usada nos testes.

## Estrutura

```text
vev/
├── playwright/       # Testes de interface e navegação web
│   ├── tests/
│   └── README.md
├── vitest/           # Teste unitário da função sum
│   └── README.md
└── README.md
```

## Ferramentas abordadas

### Playwright

Os testes ficam em `playwright/tests` e verificam o título da página do Playwright e a navegação para a página de instalação. O projeto está configurado para executar os testes em Chromium, Firefox e WebKit.

Consulte o guia de instalação e execução em [playwright/README.md](playwright/README.md).

### Vitest

O projeto contém a função `sum`, em `vitest/sum.js`, e um teste unitário que verifica se `sum(1, 2)` retorna `3`.

Consulte o guia de instalação e execução em [vitest/README.md](vitest/README.md).

## Observação

Cada ferramenta possui seu próprio `package.json` e deve ser instalada e executada a partir da respectiva pasta. Os comandos detalhados estão nos READMEs específicos.
