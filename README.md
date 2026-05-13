# Introdução ao Python

Curso de nivelamento em Python com tom acadêmico moderado, baseado em **Introduction to Computation and Programming Using Python** (John V. Guttag, MIT Press).

Pensado para preceder a pós-graduação em Visão Computacional da Sigmoidal, mas o conteúdo é autossuficiente para quem quer uma base sólida em programação com sabor de ciência da computação.

## Estrutura

4 aulas de 1h30 cada (~6h):

| Aula | Tema | Capítulos do Guttag |
|------|------|---------------------|
| 1 | Fundamentos: pensamento computacional, tipos, controle de fluxo | 1, 2, 3 (parcial) |
| 2 | Abstração: funções, escopo, estruturas de dados, mutabilidade | 4, 5, 6 (pincelada) |
| 3 | Organização: módulos, arquivos, exceções e OOP | 7, 9, 10 |
| 4 | Complexidade e algoritmos práticos: Monte Carlo e Mochila | 11, 14, 18 |

## Pré-requisitos

- Python 3.11 ou superior
- [uv](https://docs.astral.sh/uv/) (gerenciador de ambientes e dependências)

## Instalação

```bash
git clone <repo>
cd introducao-python
uv sync
```

Para abrir os notebooks:

```bash
uv run jupyter lab
```

## Organização do repo

```
introducao-python/
├── notebooks/      # Notebooks das 4 aulas
├── src/            # Módulos auxiliares (monte_carlo, mochila, etc.)
├── exercicios/     # Listas de exercícios por aula
├── data/           # Arquivos de dados (CSVs, imagens pequenas)
└── pyproject.toml  # Dependências (uv)
```

## Licença

Material didático proprietário da Sigmoidal — uso interno.
