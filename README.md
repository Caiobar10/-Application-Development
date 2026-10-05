# Verdia Tech — Site Institucional

> **Tecnologia que entende o campo.**

A **Verdia Tech** é uma startup brasileira de IoT + Inteligência Artificial para agricultura e pecuária de precisão. Ela instala sensores (umidade do solo, clima, monitoramento de rebanho) e usa IA para transformar os dados em recomendações práticas no celular do produtor: menos desperdício de água, menos perdas e decisões mais rápidas.

Este repositório contém o site institucional de uma página da empresa, feito somente com **HTML5 e CSS3**.

## Dados acadêmicos

| | |
|---|---|
| Instituição | FIAP |
| Curso | Ciência da Computação — 2º ano |
| Disciplina | Application Development |
| Professor | Allan Roberto Molto |
| Atividade | Checkpoint 2 — Site institucional (evolução da CP1) |
| Aluno | Caio Moda Francisco Fortes Barbieri |
| RM | 566747 |

## Tecnologias

- HTML5 semântico (`header`, `nav`, `main`, `section`, `article`, `aside`, `footer`)
- CSS3 externo: variáveis, Flexbox, Grid, pseudo-classes, transições e media queries
- Imagens vetoriais (SVG) próprias, sem dependências externas (a fonte Poppins tem fallback para fontes do sistema)
- Sem JavaScript e sem frameworks

## Estrutura de pastas

```
CP02_06out/
├── index.html          # página única com navegação por âncoras
├── css/
│   └── style.css       # todos os estilos, organizados em 12 blocos comentados
├── img/
│   ├── logo.svg
│   ├── hero.svg        # ilustração: campo com sensores conectados a um celular
│   ├── icone-solo.svg
│   ├── icone-rebanho.svg
│   ├── icone-clima.svg
│   └── icone-ia.svg
├── README.md
└── .gitignore
```

## Como executar

1. Abra o arquivo `index.html` diretamente no navegador **ou**
2. No VS Code, clique com o botão direito em `index.html` → **Open with Live Server** (ou **Go Live** na barra de status).

## Requisitos do enunciado → onde estão no código

| Requisito | Onde |
|---|---|
| Cabeçalho com logo/nome e menu (Início, Empresa, Soluções, Planos, Contato) | `index.html` ~linhas 32–56 · CSS bloco 5 (~linha 222) |
| Seção principal: nome, slogan, descrição, imagem | `section#inicio` ~linha 58 · CSS bloco 6 |
| Sobre a empresa: Missão, Visão e Valores | `section#empresa` ~linha 88 · CSS bloco 7 (~linha 351) |
| ≥ 3 cards com título, ícone, descrição e “Saiba mais” (4 cards) | `section#solucoes` ~linha 137 · CSS bloco 8 (~linha 393) |
| Tabela Plano / Recursos / Preço (Basic R$ 49, Pro R$ 99, Enterprise Consulte) | `section#planos` ~linha 213 · CSS bloco 9 (~linha 459) |
| Formulário: nome, e-mail, telefone, assunto, mensagem, enviar (`required`, `placeholder`, `minlength`, `maxlength`) | `section#contato` ~linha 285 · CSS bloco 10 (~linha 567) |
| Rodapé com nome, contato e links | `footer` ~linha 428 · CSS bloco 11 |
| CSS externo + variáveis | `css/style.css` bloco 1 (`:root`) |
| Box model (`box-sizing`, margin/padding/border comentados) | `css/style.css` ~linha 75 e comentários “Box model:” ao longo do arquivo |
| Layout Flexbox / Grid | Flexbox: cabeçalho, hero, cards, rodapé · Grid: missão/visão/valores, cards, contato |
| Responsividade (768px e 480px) | `css/style.css` bloco 12 (~linha 767) |

## Observação

O formulário usa `action="#"`: não há backend nesta etapa, então a validação é feita apenas pelos atributos do HTML5.
