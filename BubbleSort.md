# Introdução

Veremos como o algoritmo de ordenação Bubble Sort funciona e ver sua implementação em Java, com exemplos.

## Visão geral do Algoritmo

O Bubble Sort é um algoritmo “Algoritmo in-place”, ou seja, transforma a entrada sem nenhuma estrutura de dados auxiliar. No entanto, uma pequena quantidade de espaço de armazenamento extra é permitida para variáveis auxiliares. A entrada é geralmente substituída pela saída conforme o algoritmo é executado.

No caso do Bubble Sort ele compara a primeira posição do vetor com a segunda, caso o valor da primeira posição seja maior que o da segunda, é feito a troca de valores, caso não seja maior, o algoritmo continua a percorrer o vetor, seguindo para a segunda posição do vetor e comparando com o seguinte, repetindo o mesmo processo sucessivamente, até o fim do vetor, de forma que todo ele esteja ordenado. Quando há troca de posições, o algoritmo é “notificado”, e então, no final da iteração, o processo de ordenação é repetido novamente, até que todo o vetor esteja ordenado, e o loop de ordenação pare.

### Exemplos:

Para o exemplo, será utilizado um array não ordenado de seis elementos:

```java
int[] array = {7,4,1,2,3,10};

```
#### Iteração 1.1

Serão comparados os valores do primeiro e o segundo item da lista: 7>4? Neste caso, o primeiro valor é maior que o segundo, então haverá a troca de valores:

{4, 7, 1, 2, 3, 10}

#### Iteração 1.2

Agora serão comparados os valores do segundo e terceiro item da lista: 7>1?

{4, 1, 7, 2, 3, 10}

#### Iteração 1.3

Seguindo com as comparações: 7>2?

{4,1,2,7,3,10}

Para uma melhor experiência do processo iremos mostrar este exemplo usando Java e explicaremos o que seria essa "notificação" que o algoritmo recebe.

### Desempenho do algoritmo

No melhor caso, o algoritmo executa n operações relevantes, onde n representa o número de elementos do vetor. No pior caso, são feitas n^2 operações. A complexidade desse algoritmo é de ordem quadrática. Por isso, ele não é recomendado para programas que precisem de velocidade e operem com quantidade elevada de dados.

### Conclusão

O bubble sort é um algoritmo de ordenação que tem seu maior foco para listas que não tendam a crescer, ele é de fácil implementação como visto, e de fácil entendimento, mas no geral seu desempenho não é interessante, principalmente em listas grandes.
