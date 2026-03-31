# Projeto Educacional: Página Institucional sobre GitHub

## Visão Geral
Este projeto apresenta uma página estática sobre conceitos fundamentais do GitHub, com foco didático em:
- versionamento de código;
- colaboração entre desenvolvedores;
- organização visual de conteúdo em HTML e CSS.

A aplicação foi construída sem dependências externas, o que facilita entendimento de base para estudos de front-end.

## Objetivo
Demonstrar, em uma interface responsiva, os principais recursos do GitHub:
- Repositórios
- Pull Requests
- Issues
- Integração Contínua

## Stack e Tecnologias
- HTML5
- CSS3
- JavaScript (arquivo criado, porém sem lógica implementada no momento)

### Bibliotecas e Frameworks
Atualmente, o projeto **não utiliza bibliotecas ou frameworks externos** (ex.: Bootstrap, React, jQuery).

Impactos dessa decisão:
- menor complexidade inicial;
- carregamento mais leve;
- maior controle do CSS;
- necessidade de implementar manualmente comportamentos interativos quando necessário.

## Análise de Extensões (Ambiente de Desenvolvimento)
O projeto não depende de extensões para funcionar em produção, porém as seguintes extensões do VS Code são recomendadas para produtividade:
- Live Server: execução local com recarregamento automático.
- Prettier - Code formatter: padronização de formatação.
- HTML CSS Support: apoio de autocomplete para classes e seletores.
- ESLint (opcional): útil caso o arquivo JavaScript passe a ter regras de qualidade mais rígidas.

## Estrutura do Projeto
```text
VersionamentoVSCode/
├── index.html
├── style.css
├── script.js
└── restrito/
    └── info.txt
```

## Modelagem de Dados (Estado Atual)
Como é um front-end estático, a modelagem é simples e orientada a conteúdo renderizado:

- Dados de navegação e seções:
  - definidos diretamente no HTML (`header`, `nav`, `section`, `article`).
- Dados tabulares de exemplo (fluxo de colaboração):
  - representados em tabela HTML (`table`, `thead`, `tbody`).
- Estado da aplicação:
  - inexistente no JavaScript no momento (sem variáveis globais, sem consumo de API, sem persistência).

### Considerações de Evolução da Modelagem
Se o projeto evoluir para dados dinâmicos, recomenda-se:
- criar um arquivo JSON para conteúdos das seções;
- consumir os dados via JavaScript;
- separar camada de dados (JSON/API), apresentação (HTML/CSS) e comportamento (JS);
- adotar validação de estrutura para os dados exibidos.

## Particularidades Observadas
- Design responsivo com media query para telas menores.
- Uso de variáveis CSS em `:root`, facilitando manutenção de tema visual.
- Estrutura semântica adequada com `header`, `main`, `section`, `article` e `footer`.
- Arquivo `script.js` está vazio, indicando espaço para futuras interações.
- Pasta `restrito/` está incluída no `.gitignore`, evitando versionamento do seu conteúdo.

## Como Executar
Como é um projeto estático, há duas formas simples:

1. Abrir o arquivo `index.html` diretamente no navegador.
2. Usar a extensão Live Server no VS Code (recomendado para desenvolvimento).

## Boas Práticas Recomendadas (Próximos Passos)
- Implementar interações em `script.js` (ex.: menu mobile, animações de entrada, filtros de conteúdo).
- Criar convenção de commits (ex.: Conventional Commits).
- Adicionar linting e formatação automática no fluxo de desenvolvimento.
- Escrever testes de interface quando houver lógica JavaScript.
- Evitar armazenar dados sensíveis em arquivos locais, mesmo em diretórios ignorados.

## Licença
Projeto para fins educacionais.

Se desejar, adicione aqui uma licença formal (ex.: MIT) para uso e distribuição.
