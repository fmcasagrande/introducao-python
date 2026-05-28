# Exercícios — Aula 3

11 tarefas sobre módulos, arquivos, exceções e classes. Resolva no arquivo de sua preferência, `.py` ou `.ipynb`. Tente sem consultar a aula; se travar, volte aos exemplos.

Para a versão completa em notebook (com casos de teste e células de solução ocultas), abra `notebooks/tarefas_aula3.ipynb` ou [diretamente no Colab](https://colab.research.google.com/github/carlosfab/introducao-python/blob/main/notebooks/tarefas_aula3.ipynb).

## Parte A — Módulos e import

### 1. Distância entre dois pontos

Escreva `distancia(x1, y1, x2, y2)` que devolve a distância euclidiana entre os pontos `(x1, y1)` e `(x2, y2)`. Importe o módulo `math` e use `math.sqrt`. A fórmula é $\sqrt{(x_2 - x_1)^2 + (y_2 - y_1)^2}$.

### 2. Área e perímetro do círculo

Escreva `area_e_perimetro_circulo(raio)` que devolve uma **tupla** `(area, perimetro)`. Use `math.pi`. Lembre que a área é $\pi r^2$ e o perímetro (circunferência) é $2 \pi r$.

## Parte B — Arquivos

### 3. Salvar linhas num arquivo

Escreva `salvar_linhas(nome_arquivo, linhas)` que recebe uma lista de strings e grava cada uma numa linha do arquivo (não esqueça do `'\n'`). Use o bloco `with`.

### 4. Somar os números de um arquivo

Escreva `somar_numeros_do_arquivo(nome_arquivo)` que lê um arquivo com um número por linha e devolve a soma de todos eles. Dica: `float(linha)` converte o texto de cada linha em número.

## Parte C — Exceções e assert

### 5. Divisão segura

Escreva `divisao_segura(a, b)` que devolve `a / b`, mas devolve `None` em vez de quebrar quando `b` for zero. Use `try`/`except ZeroDivisionError`.

### 6. Conversão tolerante a erro

Escreva `para_float(texto)` que tenta converter `texto` para `float`. Se a conversão falhar, devolve `None` em vez de levantar a exceção.

### 7. Raiz quadrada com validação

Escreva `raiz_quadrada(x)` que devolve `math.sqrt(x)`, mas **levanta** um `ValueError` quando `x` for negativo. Use a instrução `raise`.

## Parte D — Classes e orientação a objetos

### 8. Classe Retangulo

Escreva a classe `Retangulo`, com `__init__(self, base, altura)` e os métodos `area()` e `perimetro()`.

### 9. Classe ContaBancaria

Escreva a classe `ContaBancaria` com saldo inicial opcional (padrão `0`). Ela deve ter `depositar(valor)`, `sacar(valor)` e `get_saldo()`. O método `sacar` deve **levantar** um `ValueError` se o valor for maior que o saldo (e, nesse caso, o saldo não muda).

### 10. Classe Ponto com dunder methods

Escreva a classe `Ponto`, com `__init__(self, x, y)` e três dunder methods: `__str__` (devolve a string `"(x, y)"`), `__eq__` (dois pontos são iguais quando têm as mesmas coordenadas) e `__add__` (soma coordenada a coordenada, devolvendo um novo `Ponto`).

### 11. Herança: Funcionario e Gerente

Escreva a classe `Funcionario`, com `__init__(self, nome, salario_base)` e o método `salario()` (que devolve o salário base). Depois escreva `Gerente(Funcionario)`, que recebe também um `bonus` no construtor (use `super().__init__`) e **sobrescreve** `salario()` para devolver salário base mais bônus.
