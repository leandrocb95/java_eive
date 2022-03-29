1. Por que a execução do Java é realizada em pilha?

R: A pilha (stack) existe para organizar a execução do código, sempre iniciada pelo médoto _main_, por ele sera acrecentado os demais médodos, sempre a cima, assim é possivel identificar o metodo que esta sendo executado, e os que esta a baixo que precisará ser executado.

2. Em programação, qual(is) a(s) utilidade(s) de *debugar* um código?

R: O Debug ajuda passar linha por linha do código, mostrando cada detalhe da execução. Por ele o desenvolvedor consegue identificar algum erro o falha.

3. Em Java, qual efeito as exceções possuem sobre o fluxo de execução da pilha? Por que, em muitos casos, o próprio desenvolvedor escreve códigos que intencionalmente lançam essas exceções?

R:Quando uma exeção e apresentada, é como acrecentar um problema em cima da pilha, impedido a execução e mudando o fluxo. A exeções podem ser inesperada ou esperadas, inesperadas quando apresenta algum erro não esperado, já esperados, são quando forçamos o esses erros.

4. O que são e qual(is) a(s) diferença(s) entre as classes `Throwable`, `Exception` e `RuntimeException`?

R: `Throwable`, `Exception` e `RuntimeException` são superclasse, derivada da classe Object. `Throwable` é mae das classes `Exception` e `RuntimeException`, que por vez, estão todos os erros e exceções na linguagem Java,`Exception` deve ser declarado o médodto throws,  `RuntimeException` não é necessário declarado o médodto throws.

5. O que são e qual(is) a(s) diferença(s) entre exceções _checked_ e _unchecked_?

R:São cetegorias de exceções,  _checked_ são verificados pelo compilador, já o _unchecked_ não são verificado pelo compilador.

6. Qual(is) a(s) diferença(s) entre uma exceção e um erro em Java?

R:Exceções são usadas em códigos. Erros são informador pela máquina virtual.

7. Explique as *keywods* `try`, `catch`, `finally`, `throw` e `throws`.

R:`try`alerta a maquina virtual, 
`catch` é definido a exeção que ira acontecer; 
`finally` utilizado para fechar conexão ou transação; 
`throw` serve para um tratamento dentro de um metodo, em uma unica exeção;
`throws` serve para um tratamento de exeção de um metodo.

8. O que é e para que serve a interface `AutoCloseable`? Como funciona o *try with resources*?

R: `AutoCloseable`é uma interface, igual a ideia de definir um contrato, caso assine deve implemnetar o metodo. *try with resources* garante o fechamento do recurso em sua finalização

9. Sobre pacotes, é correto afirmar que:

   1. É boa prática nomear os pacotes na estrutura `{site_ao_contrário}.{nome_do_projeto}`; :heavy_check_mark:
   2. Não devemos criar muitos pacotes, pois prejudica a navegação e legibilidade dentro do projeto;
   3. O uso de pacotes corretamente está diretamente relacionado à qualidade arquitetural de um projeto, já que eles servem para organizá-lo;

10. Explique a(s) diferença(s) entre os modificadores de acesso `private`, `default` `protected` e `public` em Java.

R:`private`
`default`
`protected`
`public`


11. Qual a ordem correta dos itens abaixo, considerando a estrutura de um arquivo Java onde há somente uma importação e uma classe vazia? (considere * como _wildcard_)

   ```java
   // 1

   // 2

   // 3
   ```

   1. `package *;`, `imports *;` e `class * {}`;
   2. `package *;`, `import *;` e `class * {}`; :heavy_check_mark:
   3. `pack *;`, `imports *;` e `class * {}`;
   4. `pack *;`, `import *;` e `class * {}`;



12. Explique o que é FQN (Fully Qualified Name), sua estrutura e como evitamos ter de utilizá-lo sempre que referenciamos uma classe.

R:

13. O que é, para que serve, como adquirir e como utilizar um arquivo JAR?

R:

14. O que é o pacote `java.lang` e por que ele é tão essencial para qualquer código Java?

R:

15. O que é uma `CharSequence` e qual(is) a(s) diferença(s) entre ela e uma `String`?

R:

16. Descreva os métodos da classe String citados abaixo:

    1. `.replace(char oldChar, char newChar);`
    2. `.replaceAll(String regex, String replacement)`;
    3. `.toLowerCase()`;
    4. `.concat(String str)`;
    5. `.contains(CharSequence s)`;
    6. `.equals(Object anObject)`;
    7. `.equalsIgnoreCase(String anotherString)`;
    8. `.isBlank()`;
    9. `.matches(String regex)`;

17. Qual(is) a(s) diferença(s) entre `overriding` e `overloading` de métodos? Explique-os dando exemplos úteis da aplicação de ambos.

R:

18. Todas as classes Java herdam a classe `Object`, que possui três métodos comumente sobrescritos: `.equals(Object obj)`, `.hashCode()` e `.toString()`. Explique a utilidade de cada um deles.

R:

19. Qual(is) das opções expressa(m) uma sintaxe correta para criar um *array* de inteiros?

    1. `int[] inteiros = []`;
    2. `int[] inteiros = new int[]`;
    3. `int[] inteiros = new int[]{999}`;
    4. `int[] inteiros = new int[1]`;
    5. `int[] inteiros = {999}`;
    6. `int... inteiros = {999}`;

20. Por que o primeiro código abaixo exibe o valor `0` no terminal, mas o segundo produz uma exceção?

    ```java
    // código 1
    class App {
        public static void main(String... args) {
            int[] inteiros = new int[1];
            System.out.println(inteiros[0]);
        }
    }
    ```

    ```java
    // código 2
    class Pessoa {
        Endereco endereco;
    }

    class Endereco {
        String cep;
    }

    class App {
        public static void main(String... args) {
            Pessoa[] pessoas = new Pessoa[1];
            System.out.println(pessoas[0].endereco.cep);
        }
    }
    ```

R:

21. Sobre *type casting*, explique:

    1. *Cast* implícito;
    2. *Cast* explícito;
    3. `ClassCastException`;

22. Explique o que é e como utilizar o `autoboxing` e o `unboxing`.

R:

23. É possível, no momento em que é executada uma aplicação em Java, passar argumentos para a mesma. Como isso pode ser feito e como podemos acessar esses argumentos dentro do código (no método `main()`)?

R:

24. Ao utilizar um `array`, o tamanho máximo do mesmo deve ser declarado. Por que isso não acontece quando utilizamos `ArrayList`? E qual é o limite do que essa estrutura pode armazenar?

R:

25. Por que, no geral, o `ArrayList` costuma ser mais utilizado que `arrays` em Java?

R:

26. Por que sempre devemos optar pelo uso de `Generics` ao declarar um `ArrayList` (declaração no formato `ArrayList<{tipo}>`)?

R:

27. Explique os métodos `.add(E e)` e `.contains(Object o)`, da interface `Collection`?

R:

28. Explique as interfaces `Comparator<{tipo}>` e `Comparable<{tipo}>`.

R:

29. Qual(is) a(s) diferença(s) entre as interfaces `List` e `Set`?

R:

30. Como funciona a implementação `HashSet`? Qual a relação dela com o método `.hashCode()`?

R:

31. Por que é recomendado que o *overriding* dos métodos `.equals(Object obj)` e `.hashCode()` seja realizado sempre em pares (ao sobreescrever um, o outro também deve ser sobreescrito)?

R:

32. Qual é a estrutura de uma expressão *lambda*, em Java? Explique e dê um exemplo, em código.

R:

33. Qual é a estrutura de uma expressão *lambda* utilizando *method reference*, em Java? Explique e dê um exemplo, em código.

R:

34. Qual é a estrutura de uma `stream`, em Java? Explique e dê um exemplo, em código.

R:

35. O que falta no código abaixo para ser considerado um teste útil?

    ```java
    // package & imports
    class CalculadoraTest {

    	@Test
    	public void deveSomarDoisValores() {
            Calculadora calculadora = new Calculadora();
            int resultado = calculadora.somar(2, 2);
    	}

    }
    ```
R: Esta faltando a validação, o código apresentado esta mostando a o resultado, mas falta a validação do resultado esperado, devemos utilizar o metodo 'assert', que nos permite verificar se comportamento é o esperado.

36. Como é aplicado o TDD? Qual(is) benefício(s) ele traz e quando devemos utilizá-lo?

R: O TDD (Teste Driven Development) é aplicado por Testes >> Implementação >> Refatutação. Para códigos mais elaborados é recomendavel inicar pelos teste, antes mesmo de inciar o código, pois dessa maneiras o código ficará mais simples, impelmentando ele a nececidades dos teste, sendo possivel refaturar, ou seja, enxugando e deixando o cógigo fácil a manutenção.

37. Quais métodos podemos utilizar para validar o lançamento de exceções em testes automatizados?

