# Pares na soma dos números naturais

Este repositório contém um pequeno experimento computacional em Python
inspirado por uma observação simples sobre a soma da sequência dos números naturais.

A ideia central é relacionar a soma da sequência {0, 1, 2, ..., n} com a quantidade
de pares distintos de números naturais (a, b), tais que a + b = n.

O código aqui apresentado não tem como objetivo otimização ou formalismo matemático,
mas sim ilustrar de forma concreta e verificável uma inferência simples e intuitiva.

Este código acompanha o artigo publicado no Medium:

👉 [Errar somas, encontrar padrões](https://medium.com/@GilPedrosoJr./errar-somas-encontrar-padr%C3%B5es-bf3175d2e06f)

---

## Motivação

Ao realizar manualmente somas da forma:

0 + 1 + 2 + 3 + ... + n

surge naturalmente a possibilidade de reorganizar os termos em pares que somam
exatamente o último elemento da sequência. A partir dessa reorganização,
observa-se que a quantidade desses pares está diretamente relacionada com
a soma total da sequência.

Este repositório acompanha essa observação por meio de um pequeno script em Python,
permitindo que qualquer leitor teste exemplos diferentes e verifique o padrão.

---

## Descrição da observação

Dada a sequência {0, 1, 2, ..., n}, consideram-se pares distintos (a, b) tais que:

- a < b  
- a + b = n  

A soma total da sequência é dada por:

S = 0 + 1 + 2 + ... + n = n(n + 1) / 2

Define-se j como a quantidade máxima de pares distintos cuja soma resulta em n.
Esse valor corresponde ao maior inteiro tal que:

j · n ≤ S

Equivalentemente:

j ≤ (n + 1) / 2

Como j representa uma quantidade de pares, ele deve ser inteiro. Assim, de forma
mais precisa:

j = ⌊(n + 1) / 2⌋

O código implementa exatamente essa contagem e exibe explicitamente os pares encontrados.

---

## Como utilizar

Certifique-se de ter o Python instalado (versão 3.x).

Execute o script no terminal:

```bash
python pares_soma.py
```
ou simplesmente copie o código e rode em algum meio de sua preferência.
