# Introdução ao Python

Curso de nivelamento em Python com tom acadêmico moderado, baseado em **Introduction to Computation and Programming Using Python** (John V. Guttag, MIT Press) e nas lectures de Ana Bell em **MIT 6.100L**.

Uma realização **Sigmoidal** e **STAR Research Institute**. Pensado para preceder a pós-graduação em Visão Computacional.

## Cronograma

4 aulas ao vivo, sempre nas **quartas-feiras das 20h às 22h** (horário de Brasília):

| Aula | Data | Tema |
|------|------|------|
| 1 | 13/05 | Fundamentos e pensamento computacional |
| 2 | 20/05 | Abstração: funções, escopo, estruturas de dados |
| 3 | 27/05 | Organização: módulos, arquivos, exceções e OOP |
| 4 | 03/06 | Complexidade e algoritmos práticos |

> As aulas da pós em Visão Computacional, no calendário regular, começam em **10/06**.

## Ementa detalhada

### Aula 1 — Fundamentos e pensamento computacional
Capítulos 1, 2, 3 (parcial) do Guttag.

- O que é computação: conhecimento declarativo vs imperativo, algoritmo como receita.
- Python como calculadora: tipos primitivos `int`, `float`, `str`, `bool`.
- Variáveis e *binding*: a variável como rótulo, não como caixa.
- Branching: `if`, `elif`, `else`, indentação como sintaxe.
- Iteração: `while`, `for`, `range`.
- Primeiro mergulho algorítmico: enumeração exaustiva e busca por bisseção.

### Aula 2 — Abstração: funções, escopo e estruturas de dados
Capítulos 4, 5 e introdução do 6 do Guttag.

- Funções: parâmetros, retorno, escopo, abstração.
- Listas, tuplas, dicionários e strings.
- Slicing, indexação e operações comuns sobre sequências.
- Mutabilidade e *aliasing* (a fonte mais comum de bugs em Python científico).
- Recursão como conceito.

### Aula 3 — Organização de código
Capítulos 7, 9 e 10 do Guttag.

- Módulos e `import`; organização de projeto.
- Leitura e escrita de arquivos.
- Exceções e `assert`.
- Classes e orientação a objetos: atributos, métodos, herança, *dunder methods*.

### Aula 4 — Complexidade e algoritmos práticos
Capítulos 11, 14 e 18 do Guttag.

- Complexidade algorítmica: notação O grande na prática, demonstrada com medições de tempo.
- **Monte Carlo**: estimando π com pontos aleatórios e plotando a convergência.
- **Problema da Mochila**: brute force vs greedy, ótimo vs aproximação.
- Ponte para Visão Computacional: imagem como array de números.

## Como acompanhar as aulas

Você tem **dois caminhos**. Os dois funcionam — escolha o que faz mais sentido para seu momento.

### Caminho A: Google Colab (zero instalação)

Se está saindo do zero e quer começar **agora**, sem se preocupar com instalação:

1. Baixe o arquivo `.ipynb` da aula desta pasta `notebooks/` (botão *Download raw file* no GitHub).
2. Acesse [colab.research.google.com](https://colab.research.google.com).
3. *File → Upload notebook* e selecione o `.ipynb` baixado.
4. Pronto — pode rodar célula por célula durante a aula.

Funciona em qualquer computador com navegador, inclusive Chromebook.

### Caminho B: ambiente local (recomendado a partir da Aula 2)

Para ter um ambiente "de verdade", igual ao que você vai usar no dia a dia profissional:

```bash
# 1. Clone este repositório
git clone <url-do-repo>
cd introducao-python

# 2. Instale as dependências com uv
uv sync

# 3. Abra os notebooks
uv run jupyter lab
```

Pré-requisitos: **Python 3.11+** e **[uv](https://docs.astral.sh/uv/getting-started/installation/)**.

## Tarefa de preparação para a Aula 2

Para começarmos a Aula 2 com todo mundo no mesmo ambiente, **instale Python e escolha uma IDE até quarta que vem**. É a primeira tarefa prática do curso.

### 1. Instalar Python

- **Windows** — baixe o instalador oficial em [python.org/downloads](https://www.python.org/downloads/) e, no instalador, **marque a opção "Add Python to PATH"** antes de clicar em *Install Now*. Para verificar, abra o PowerShell e rode `python --version`.
- **macOS** — já vem com Python pré-instalado. Para verificar, abra o Terminal e rode `python3 --version`. Se a versão for inferior a 3.11, instale uma mais recente via [python.org/downloads](https://www.python.org/downloads/) ou `brew install python`.
- **Linux** — quase todas as distribuições já trazem Python. Verifique com `python3 --version` no terminal. Se precisar atualizar, use o gerenciador da sua distribuição.

### 2. Escolher uma IDE (ou editor de código)

Uma IDE é o ambiente onde você vai escrever e rodar seus programas. Sugestões em ordem de recomendação para iniciantes:

| Editor | Quando faz sentido | Link |
|--------|--------------------|------|
| **Antigravity** | Para quem quer experimentar uma IDE moderna com IA integrada nativamente. | [antigravity.google](https://antigravity.google/) |
| **Cursor** | Similar ao VS Code, com IA por padrão. Boa curva de aprendizado. | [cursor.com](https://cursor.com/) |
| **VS Code** | Padrão de mercado, gratuito, leve. Funciona em qualquer máquina. | [code.visualstudio.com](https://code.visualstudio.com/) |
| **PyCharm Community** | Mais robusto, mais "pesado". Bom para projetos grandes. | [jetbrains.com/pycharm](https://www.jetbrains.com/pycharm/) |

Escolha **uma** e instale. Não tem certo ou errado — qualquer uma serve para o curso inteiro. Se nunca usou IDE alguma, comece pelo **Antigravity** ou **VS Code**.

### 3. (Opcional) Instalar o uv

O `uv` é o gerenciador de ambientes que usamos no repositório. Não é obrigatório para acompanhar — mas se quiser entrar no Caminho B (ambiente local), instale-o seguindo as [instruções oficiais](https://docs.astral.sh/uv/getting-started/installation/).

## Organização do repositório

```
introducao-python/
├── notebooks/      # Notebooks das 4 aulas
├── src/            # Módulos auxiliares (monte_carlo, mochila, etc.)
├── exercicios/     # Listas de exercícios por aula
├── data/           # Arquivos de dados (CSVs, imagens pequenas)
└── pyproject.toml  # Dependências (uv)
```

## Referências

- Guttag, J. V. *Introduction to Computation and Programming Using Python*. 3rd ed. MIT Press, 2021.
- Bell, A. *MIT 6.100L — Introduction to Computer Science and Programming Using Python*, Fall 2022. Disponível no [MIT OpenCourseWare](https://ocw.mit.edu/courses/6-100l-introduction-to-cs-and-programming-using-python-fall-2022/).

## Licença

Material didático proprietário — Sigmoidal e STAR Research Institute. Uso interno.
