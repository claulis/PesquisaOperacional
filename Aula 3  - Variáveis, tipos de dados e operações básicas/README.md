# 1. Variáveis
Variáveis são elementos fundamentais em programação que servem para armazenar e manipular dados dentro de um programa. Elas funcionam como "caixas" onde você pode **guardar informações** que podem ser utilizadas e modificadas durante a execução do programa.

Para explicar melhor, imagine uma caixa onde você pode colocar diferentes tipos de objetos, como números, textos, listas, etc. Cada caixa tem um nome único que permite acessar o conteúdo armazenado dentro dela.

Aqui estão os principais pontos sobre variáveis:

1. **Armazenamento de Dados**: As variáveis **armazenam diferentes tipos de dados**, como números, textos, booleanos (verdadeiro ou falso), listas, entre outros.

2. **Nomeação Única**: Cada variável tem um **nome único** que é usado para acessar e manipular seu conteúdo dentro do programa.
> :warning: Não podem ter duas variáveis com mesmo nome (cuidado com maiúscolas/minúscolas)

3. **Flexibilidade de Conteúdo**: As variáveis podem armazenar **diferentes tipos de dados ao longo da execução do programa**. Por exemplo, uma variável pode armazenar um número em um momento e uma string (texto) em outro momento.

4. **Manipulação de Dados**: Você pode manipular o conteúdo das variáveis de várias maneiras, como atribuir novos valores, realizar operações matemáticas, concatenar strings, entre outras operações, dependendo do tipo de dado armazenado na variável.

5. **Escopo**: O escopo de uma variável determina **onde ela pode ser acessada dentro do programa**. Existem *variáveis locais*, que são acessíveis apenas dentro de uma determinada função ou bloco de código, e *variáveis globais*, que podem ser acessadas de qualquer lugar no programa.

Quando começar a aprender programação, você usará variáveis o tempo todo, pois são essenciais para armazenar e manipular dados. Aqui estão algumas situações comuns em que você usaria variáveis:

- **Armazenar informações do usuário**: Por exemplo, ao criar um programa de cadastro, você pode armazenar o nome, idade e outras informações fornecidas pelo usuário em variáveis para processamento posterior.
- **Realizar cálculos**: Variáveis são usadas para armazenar resultados intermediários ou finais de cálculos matemáticos ou lógicos.
- **Iteração e controle de fluxo**: Em estruturas de repetição (loops) ou em condicionais, você usará variáveis para controlar o fluxo do programa, como contadores em loops ou variáveis de condição em estruturas condicionais.
- **Manipulação de texto**: Variáveis são amplamente utilizadas para armazenar e manipular texto, como mensagens de saída, entrada do usuário, etc.

# 2. Variáveis em Python

Em Python, as variáveis são bastante simples e flexíveis. Aqui estão os conceitos básicos sobre variáveis em Python:

1. **Declaração de Variáveis**: Em Python, você declara uma variável atribuindo um valor a ela. *Não é necessário declarar explicitamente o tipo da variável*, pois Python é uma linguagem de tipagem dinâmica.

    ```python
    # Exemplo de declaração de variáveis
    idade = 25
    nome = "João"
    salario = 1500.50
    ```

2. **Tipos de Dados Dinâmicos**: As variáveis em Python podem *armazenar qualquer tipo de dado, e o tipo de dado pode ser alterado simplesmente atribuindo um novo valor à variável*.


3. **Nomes de Variáveis**: Os nomes de variáveis em Python devem seguir algumas regras:
  >:warning: Importante :point_down:
  > - Devem começar com uma letra (a - z, A - Z) ou um sublinhado (_).
  > - Podem conter letras, números e sublinhados.
  > - Não podem começar com números.
  > - Python faz distinção entre maiúsculas e minúsculas, ou seja,  "nome" e "Nome" são considerados nomes de variáveis diferentes.

4. **Imutabilidade de Alguns Tipos de Dados**: Alguns tipos de dados em Python, como **strings, tuplas e números imutáveis (como int, float)**, não podem ser alterados depois de criados. Isso significa que quando você faz uma operação em uma variável desse tipo, **na verdade você está criando uma nova variável com o valor modificado**.

5. **Escopo de Variáveis**: As variáveis em Python têm escopos locais e globais. Se uma variável é definida dentro de uma função, ela é local a essa função. Se for definida fora de todas as funções, ela é global.

   ```python
   x = 10  # Variável global

   def minha_funcao():
       y = 20  # Variável local
       print(x)  # Acesso à variável global

   minha_funcao()
   ```

6. **Convenções de Nomenclatura**: Em Python, é comum seguir as convenções de nomenclatura PEP8, que sugerem o uso de letras minúsculas para nomes de variáveis, separadas por sublinhados em caso de nomes compostos.

   ```python
   nome_completo = "João Silva"
   salario_mensal = 1500.50
   ```

# 3. Tipos de dados

Em Python, existem vários tipos de dados que podem ser usados para representar diferentes tipos de informações. Abaixo estão alguns dos tipos de dados mais comuns em Python, juntamente com exemplos de cada um:

1. **Inteiros (int)**: Representam números inteiros, positivos ou negativos, sem parte fracionária.

```python
idade = 30
ano_nascimento = 1992
```

2. **Números de Ponto Flutuante (float)**: Representam números reais, incluindo números com parte fracionária.

```python
altura = 1.75
peso = 68.5
```

3. **Booleanos (bool)**: Representam valores lógicos Verdadeiro (True) ou Falso (False).

```python
temperatura_alta = True
dia_ensolarado = False
```

4. **Strings (str)**: Representam sequências de caracteres, como texto.

```python
nome = "Maria"
endereco = 'Rua Principal, 123'
```

5. **Listas (list)**: São coleções ordenadas de itens, onde cada item pode ser de qualquer tipo de dado, inclusive outra lista.

```python
numeros = [1, 2, 3, 4, 5]
nomes = ["João", "Maria", "Pedro"]
```

6. **Tuplas (tuple)**: São semelhantes às listas, mas são imutáveis, ou seja, uma vez criadas, não podem ser alteradas.

```python
coordenadas = (10, 20)
cores_rgb = ('vermelho', 'verde', 'azul')
```

7. **Dicionários (dict)**: São coleções de pares chave-valor, onde cada valor é acessado por uma chave única.

```python
pessoa = {'nome': 'Ana', 'idade': 25, 'cidade': 'São Paulo'}
```

8. **Conjuntos (set)**: São coleções não ordenadas de elementos únicos. Conjuntos são úteis quando você quer elementos únicos e não precisa se preocupar com a ordem.

```python
vogais = {'a', 'e', 'i', 'o', 'u'}
```

# 4. Operações básicas

Vamos criar exemplos simples de operações com cada tipo de dados em Python:

1. **Operações com Inteiros (int)**:

```python
# Adição
soma = 10 + 5
print(soma)  # Saída: 15

# Subtração
diferenca = 20 - 8
print(diferenca)  # Saída: 12

# Multiplicação
produto = 6 * 4
print(produto)  # Saída: 24

# Divisão
quociente = 100 / 5
print(quociente)  # Saída: 20

# Potência
potencia = 2 ** 3
print(potencia)  # Saída: 8
```

2. **Operações com Números de Ponto Flutuante (float)**:

```python
# Adição
soma = 3.5 + 2.5
print(soma)  # Saída: 6.0

# Subtração
diferenca = 10.8 - 4.3
print(diferenca)  # Saída: 6.5

# Multiplicação
produto = 3.14 * 2
print(produto)  # Saída: 6.28

# Divisão
quociente = 15 / 2
print(quociente)  # Saída: 7.5

# Potência
potencia = 2.5 ** 2
print(potencia)  # Saída: 6.25
```

3. **Operações com Booleanos (bool)**:

```python
# Operações lógicas
verdadeiro = True
falso = False

# Operador AND
resultado_and = verdadeiro and falso
print(resultado_and)  # Saída: False

# Operador OR
resultado_or = verdadeiro or falso
print(resultado_or)  # Saída: True

# Operador NOT
resultado_not = not verdadeiro
print(resultado_not)  # Saída: False
```

4. **Operações com Strings (str)**:

```python
# Concatenação
saudacao = "Olá, "
nome = "Maria"
mensagem = saudacao + nome
print(mensagem)  # Saída: Olá, Maria

# Acesso a caracteres
primeira_letra = nome[0]
print(primeira_letra)  # Saída: M

# Tamanho da string
tamanho_nome = len(nome)
print(tamanho_nome)  # Saída: 5
```

5. **Operações com Listas (list)**:

```python
# Adição de elementos
numeros = [1, 2, 3]
numeros.append(4)
print(numeros)  # Saída: [1, 2, 3, 4]

# Acesso a elementos
primeiro_numero = numeros[0]
print(primeiro_numero)  # Saída: 1

# Tamanho da lista
tamanho_numeros = len(numeros)
print(tamanho_numeros)  # Saída: 4
```

