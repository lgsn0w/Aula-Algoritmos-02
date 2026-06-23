# Aula-Algoritmos-02 — Estrutura de Repetição `para`

## Sobre

Este repositório contém material da **Aula 02 de Algoritmos**, focada na estrutura de repetição `para` (equivalente ao `for` em linguagens como C, Java e Python). Os algoritmos foram escritos em **VisuAlg** (pseudocódigo em português).

---

## O que é o `para`?

O `para` é uma estrutura de repetição **com contador**. Ele é usado quando sabemos **exatamente quantas vezes** o bloco de código precisa ser executado.

### Sintaxe

```
para <variável> de <início> ate <fim> faca
   // comandos que se repetem
fimpara
```

| Elemento | Descrição |
|---|---|
| `variável` | O contador que controla a repetição (geralmente `i`) |
| `de <início>` | Valor inicial do contador |
| `ate <fim>` | Valor final — o loop para quando o contador ultrapassa esse valor |
| `faca` / `fimpara` | Delimitam o bloco de comandos que será repetido |

A cada iteração, a variável é **incrementada automaticamente em 1**.

### Quando usar o `para`?

- Quando o **número de repetições é conhecido** antes do loop começar.
- Exemplos: percorrer uma lista de N alunos, calcular tabuada de 1 a 10, somar N notas.

> Se o número de repetições **não é conhecido** antecipadamente (ex: repetir até o usuário digitar 0), usa-se `enquanto` ou `repita` em vez do `para`.

---

## Algoritmos do Repositório

### 1. `algoritmo SomaEMedia.alg`

Calcula a **soma e a média** de N notas digitadas pelo usuário.

**Fluxo:**
1. Pergunta quantas notas serão digitadas (`n`).
2. Usa `para i de 1 ate n faca` para ler cada nota e acumular na variável `soma`.
3. Após o loop, calcula `media <- soma / n` e exibe os resultados.

**Exemplo de execução (n = 3):**

```
Quantas notas voce quer digitar?
3
Digite a nota 1:
7.5
Digite a nota 2:
8.0
Digite a nota 3:
6.0
Soma das notas: 21.5
Media da turma: 7.17
```

O `para` é ideal aqui porque o usuário define `n` antes do loop — o número de repetições é conhecido.

---

### 2. `algoritmo Tabuada.alg`

Gera a **tabuada** de um número inteiro digitado pelo usuário (de 1 a 10).

**Fluxo:**
1. Lê o número do usuário.
2. Usa `para i de 1 ate 10 faca` para multiplicar o número por cada valor de `i`.
3. Exibe cada linha no formato `numero x i = resultado`.

**Exemplo de execução (numero = 7):**

```
Digite um numero inteiro:
7
7 x 1 = 7
7 x 2 = 14
7 x 3 = 21
7 x 4 = 28
7 x 5 = 35
7 x 6 = 42
7 x 7 = 49
7 x 8 = 56
7 x 9 = 63
7 x 10 = 70
```

Aqui o `para` é perfeito porque a tabuada sempre vai de 1 a 10 — número fixo de iterações.

---

## Material de Apoio

- **[`topico1_para.pdf`](topico1_para.pdf)** — Slides da aula sobre a estrutura `para` (PDF).
- **`topico1_para.pptx`** — Versão editável dos slides (PowerPoint).

## Como Executar

1. Baixe e instale o [VisuAlg](https://visualg3.com.br/).
2. Abra um dos arquivos `.alg` no VisuAlg.
3. Pressione **F9** para executar o algoritmo.
