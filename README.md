# Exibição de Elementos de um Vetor de Strings em Java

Este projeto consiste em um programa Java simples que demonstra duas maneiras comuns de percorrer e exibir os elementos de um array (vetor) de strings.

**Autor:** gustavodees

## Arquivos Incluídos

* `principal/Main.java`: Contém a classe principal com o método `main`, onde as duas formas de iteração sobre o array são demonstradas.

## Como Usar

1.  **Salve o arquivo:** Salve o código fornecido em um arquivo chamado `Main.java` dentro de uma pasta chamada `principal`.
2.  **Compile o código:** Abra um terminal ou prompt de comando, navegue até o diretório raiz do seu projeto e compile o arquivo Java utilizando o compilador Java:

    ```bash
    javac principal/Main.java
    ```

3.  **Execute o programa:** Após a compilação ser concluída com sucesso, execute a classe `Main` com o comando:

    ```bash
    java principal.Main
    ```

4.  **Resultado:** O programa exibirá o nome de cada pessoa contida no array `vect`, primeiro utilizando um loop `for` tradicional e depois utilizando um loop `for-each` (ou "for aprimorado"). As duas formas de iteração produzirão a mesma saída, com os nomes "Maria", "Bob" e "Alex" sendo impressos cada um em sua própria linha, separados por uma linha de "##################".

## Explicação do Código

### `principal/Main.java`

Este arquivo contém a classe `Main`, que é o ponto de entrada do programa.

* **Método `main`:**
    1.  Cria e inicializa um array de strings chamado `vect` com três elementos: "Maria", "Bob" e "Alex".
    2.  **Primeiro Loop (for tradicional):**
        * Utiliza um loop `for` tradicional que itera através do array `vect` usando um índice inteiro `i`, que começa em 0 e vai até o tamanho do array menos 1.
        * Em cada iteração, o elemento do array na posição do índice `i` (`vect[i]`) é acessado e impresso no console utilizando `System.out.println()`.
    3.  Imprime uma linha separadora "##################" para distinguir a saída dos dois loops.
    4.  **Segundo Loop (for-each ou for aprimorado):**
        * Utiliza um loop `for-each`, também conhecido como "for aprimorado". A sintaxe `for (String obj : vect)` significa "para cada objeto String chamado `obj` dentro do array `vect`".
        * Este tipo de loop simplifica a iteração sobre coleções (como arrays) e diretamente acessa cada elemento do array sem a necessidade de um índice explícito.
        * Em cada iteração, a variável `obj` assume o valor do elemento atual do array, que é então impresso no console.

Este programa demonstra duas maneiras equivalentes de percorrer todos os elementos de um array em Java. O loop `for` tradicional oferece mais controle sobre o índice, enquanto o loop `for-each` geralmente é mais conciso e legível para simplesmente iterar sobre todos os elementos de uma coleção.
