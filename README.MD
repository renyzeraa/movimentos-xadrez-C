# README - Simulação de Movimentos no Xadrez

Este programa em C simula os movimentos de quatro peças do xadrez: **Torre, Bispo, Rainha e Cavalo**. O código utiliza recursividade para algumas peças e loops aninhados para outras, garantindo um código eficiente e bem estruturado.

## Estrutura do Programa

O programa está dividido em quatro seções, cada uma simulando o movimento de uma peça de xadrez:

### 1. **Movimento da Torre** (Recursividade)

- A Torre se move apenas na horizontal.
- O movimento é implementado por uma **função recursiva** chamada `moverTorre(int movimentos)`.
- A função imprime "Direita" e chama a si mesma até atingir o número desejado de movimentos.

### 2. **Movimento do Bispo** (Recursividade + Loop Aninhado)

- O Bispo se move na diagonal, combinando os movimentos "Cima" e "Direita".
- A função `moverBispo(int movimentos)` utiliza um **loop interno** para simular o movimento diagonal e depois chama a si mesma recursivamente.

### 3. **Movimento da Rainha** (Recursividade)

- A Rainha pode se mover em qualquer direção, mas aqui simulamos apenas um movimento para a esquerda.
- A função `moverRainha(int movimentos)` imprime "Esquerda" e se chama recursivamente até atingir o número desejado de movimentos.

### 4. **Movimento do Cavalo** (Loops Aninhados + Controle de Fluxo)

- O Cavalo se move em "L", ou seja, duas casas em uma direção e uma casa perpendicular.
- A implementação utiliza **loops aninhados** para simular o movimento "Cima" e depois "Direita".
- Utiliza uma condicional `if` para garantir que o movimento para a direita ocorra apenas após os dois movimentos para cima.

## Execução

O programa exibe no console a sequência exata de movimentos para cada peça, separando-os com espaços em branco para facilitar a leitura.

## Exemplo de Saída

```
Movimento da Torre:
Direita
Direita
Direita
Direita
Direita

Movimento do Bispo:
Cima, Direita
Cima, Direita
Cima, Direita
Cima, Direita
Cima, Direita

Movimento da Rainha:
Esquerda
Esquerda
Esquerda
Esquerda
Esquerda
Esquerda
Esquerda
Esquerda

Movimento do Cavalo:
Cima
Cima
Direita
```

## Melhorias Implementadas

✅ Uso de **recursividade** para a Torre, Bispo e Rainha.
✅ Uso de **loops aninhados** para o movimento do Cavalo e Bispo.
✅ Uso de **condicionais (if)** para melhorar a precisão do movimento do Cavalo.
✅ **Código eficiente**, evitando chamadas recursivas desnecessárias para evitar estouro de pilha.
✅ **Legibilidade aprimorada** com indentação adequada e nomes descritivos de variáveis.

## Como Compilar e Executar

Para compilar o programa, use um compilador como `gcc`:

```sh
gcc -o xadrez xadrez.c
./xadrez
```

## Conclusão

Este programa demonstra como utilizar recursividade, loops aninhados e controle de fluxo para simular movimentos no xadrez. Ele pode ser expandido para incluir outras peças e estratégias avançadas de movimento.

🚀 **Desenvolvido para estudo e prática de C!**
