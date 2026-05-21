# Exercícios — Aula 2

10 tarefas sobre funções, listas, mutabilidade, tuplas, strings, dicionários e recursão. Resolva no arquivo de sua preferência — `.py` ou `.ipynb`. Tente sem consultar a aula; se travar, volte aos exemplos.

## Parte A — Funções

### 1. Conversor Celsius → Fahrenheit

Escreva `celsius_para_fahrenheit(c)` que devolve `c * 9/5 + 32`.

### 2. Maior entre três números

Escreva `maior_de_tres(a, b, c)` que devolve o maior dos três sem usar `max`.

## Parte B — Listas e mutabilidade

### 3. Soma dos elementos

Escreva `soma_lista(lista)` que devolve a soma de todos os elementos. Não use `sum`. Cuidado com a lista vazia (resultado: `0`).

### 4. Maior elemento

Escreva `maior_elemento(lista)` que devolve o maior número de uma lista não vazia, sem usar `max`.

### 5. Dobrar valores sem alterar a original

Escreva `dobrar(lista)` que devolve uma **nova lista** com cada elemento multiplicado por 2 — a lista original **não pode ser alterada**. Lembre que `nova = lista` é alias; use `lista[:]` se quiser cópia.

## Parte C — Strings, tuplas e dicionários

### 6. Inverter string sem `[::-1]`

Escreva `inverter(s)` que devolve a string ao contrário usando um `for`.

### 7. Mínimo e máximo numa tupla

Escreva `min_max(lista)` que devolve uma tupla `(menor, maior)` sem usar `min` nem `max`.

### 8. Frequência de caracteres

Escreva `frequencia(s)` que devolve um dicionário com a contagem de cada caractere. (Mesmo padrão do exemplo da aula com `'visao_computacional'`.)

## Parte D — Recursão

### 9. Soma de 1 até `n` (recursiva)

Escreva `soma_ate(n)` que devolve $1 + 2 + \ldots + n$ de forma recursiva. Caso base: `n <= 1` devolve `n`.

### 10. Potência recursiva *(desafio)*

Escreva `potencia(base, expoente)` que devolve `base` elevado a `expoente`, sem usar `**` nem `math.pow`. Assuma `expoente >= 0`. Caso base: qualquer número elevado a `0` é `1`.
