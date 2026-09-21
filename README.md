# QuickSort em Java

Implementação do algoritmo de ordenação **QuickSort**, usando a estratégia de divisão e conquista.

## Como funciona

1. Escolhe um elemento do array como **pivô** (neste caso, o último elemento).
2. **Particiona** o array: valores menores que o pivô vão para a esquerda, maiores vão para a direita.
3. Aplica o mesmo processo **recursivamente** em cada partição, até o array estar totalmente ordenado.

## Complexidade

| Caso        | Tempo       |
|-------------|-------------|
| Melhor caso | O(n log n)  |
| Caso médio  | O(n log n)  |
| Pior caso   | O(n²)       |
| Espaço      | O(log n)    |

O pior caso acontece quando o array já está ordenado (ou quase), pois o pivô escolhido acaba sendo sempre o menor ou o maior valor.

## Como executar

Compile e rode o arquivo com o JDK instalado:

```bash
javac QuickSort.java
java QuickSort
```

### Saída esperada

```
Array original: [9, 3, 7, 1, 8, 2, 5, 4, 6]
Array ordenado: [1, 2, 3, 4, 5, 6, 7, 8, 9]
```

## Estrutura do código

- `sort(int[] array)` — método público, ponto de entrada do algoritmo.
- `quickSort(...)` — controla a recursão sobre as partições.
- `particionar(...)` — organiza os elementos em torno do pivô.
- `trocar(...)` — troca dois elementos de posição no array.

## Requisitos

- JDK 8 ou superior.
