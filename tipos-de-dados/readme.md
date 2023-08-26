# Variáveis e Tipos de dados

Python é uma linguagem de tipagem forte e dinâmica. Essa característica está relacionada à forma como os tipos de dados são tratados durante a execução do código. Vamos entender o que isso siginifica:

## **Tipagem forte:**

A tipagem forte refere-se ao fato de que em Python, os tipos de dados são rigorosamente mantidos e não são implicitamente convertidos para outros tipos de dados. Isso siginifica que você não pode realizar operações entre tipos de dados incompatíveis sem fazer conversões explícitas.

Por exemplo, em python, você não pode somar uma String com um número diretamente, sem fazer uma conversão. Isso é diferente de linguagens de tipagem fraca, onde as conversões podem acontecer automaticamente, o que às vezes pode levar a resultados inesperados.

**código exemplo**:

```python
# Isso resultará em um erro:
idade = 25
print(f"Sua idade é" + idade)
```

## **Tipagem dinâmica:**

A tipagem dinâmica refere-se à capacidade do Python determinar o tipo de uma variávem em tempo de execução, isto permite que você atribua diferentes tipos de dados a uma mesma variável ao longo do tempo. Ou seja, você não precisa declarar explicitamente o tipo de uma variável no momento da criação:

```python
# Não é necessário declarar explicitamente o tipo
x = 5      # x é um inteiro
x = "hello"  # x agora é uma string
x = [1, 2, 3]  # x agora é uma lista
```

Em resumo, a combinação de tipagem forte e dinâmica em Python significa que os tipos de dados são rigorosamente mantidos e que a linguagem é capaz de inferir o tipo de uma variável durante a execução, tornando-a flexível, porém cuidadosa na manipulação dos tipos de dados.

## Tipos de dados

### Dados básicos

* Inteiro
  * ```python
    idade = 25
    print("# Inteiro")
    print(str(idade))
    ```
* Ponto Flutuante
  * ```python
    # Ponto flutuante
    altura = 1.75
    print("# Ponto flutuante")
    print(str(altura))
    ```
* String
  * ```python
    # String
    nome = 'Jhonatas'
    print("# String")
    print(nome)
    ```
* Boolane
  * ```python
    # Booleano
    tem_carro = False
    print("# Booleano")
    print(tem_carro)
    ```
* None Type
  * ```python
    # None Type
    valor = None
    ```

### Estrutura de dados

#### Listas

É uma coleção, ordenada e mutável de elementos que pode ser formada, por diferentes tipos.

**Sua Sintaxe é : `[elemento1, elemento2, elemento3]`**

**Principais operações:**

* Como instanciar uma lista
  * ```python
    numeros = [1, 2, 3, 4, 5]
    ```
* Acessar pelo índice
  * ```
    primeiro_numero = numeros[0]
    ultimo_numero = numeros[-1]
    ```
* Adicionar elementos pelo índice
  * ```python
    numeros.append(9) # Adiciona ao final
    numeros.insert(2,7) # Aceita dos parãmetros índice e valor
    ```
* Remover
  * ```python
    numeros.remove(3) # Remove o elemento pelo valor
    numero_removido = numeros.pop() # Remove e retorna o ultimo elemento
    ```
* Atualizar pelo índice
  * ```python
    numeros[0] = 0
    ```
* Tamanho da lista
  * ```python
    tamanho = len(numeros)
    ```
* Ordenar a lista
  * ```python-repl
    numeros.sort()
    ```
* Iterar pela lista
  * ```python-repl
    for numero in numeros:
        print(numero)
    ```

#### Tuplas


É uma coleção ordenada e imutável de elementos

Geralmente usada quando se deseja armazenar um conjunto d evalores que não devem ser alterados

Sintaxe `(elemento1, elemento2, elemento3)`
