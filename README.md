# curso-react-native-1.0


1 - Primeiros passos no curso
    * Apresentação do curso
    * Repositório do curso
    * Duvidas e sugestões de novos videos para o curso
        - Serão feitas durante o curso como bónus 

2 - Preparando ambiente de desenvolvimento linux
    * Instalando o java
        - https://www.linuxcapable.com/how-to-install-oracle-java-17-on-linux-mint/
    * Instalando Node JS
        - https://github.com/nodesource/distributions?tab=readme-ov-file#ubuntu-versions
    * Download android studio
        - https://developer.android.com/studio?_gl=1*1gmr7jf*_up*MQ..&gclid=CjwKCAiA29auBhBxEiwAnKcSqkU9ILsdkNvcPhBY_RWP23mu1UnWYZd5D7_Aw0WWqwNXIdUf1t03KhoCf8EQAvD_BwE&gclsrc=aw.ds&hl=pt-br
    * Instalando o android studio
        - https://developer.android.com/studio/install?gad_source=1&gclid=CjwKCAiA29auBhBxEiwAnKcSqkU9ILsdkNvcPhBY_RWP23mu1UnWYZd5D7_Aw0WWqwNXIdUf1t03KhoCf8EQAvD_BwE&gclsrc=aw.ds
    * Dica após instalação
        - Tip: To make Android Studio available in your list of applications, select Tools > Create Desktop Entry from the Android Studio menu bar.
    * Configurações do react-native
        - https://reactnative.dev/docs/environment-setup

3 - Editor de código fonte
    * Instalando o vs code e adicionando plugin expo

4 - Adquerindo conhecimentos basicos em javascript
    * Comentários
        - Comentários de uma linha 
            - // Comentário teste
            - let x = 5; // Esta linha declara uma variável 'x' com o valor 5
        - Comentários de várias linhas
            - 
                /* Este é um comentário
                    de várias linhas
                */
    * Variáveis
        * Declarando Variáveis
            - var: Era a forma antiga de declarar variáveis em JavaScript. É globalmente escopo ou escopo de função, não escopo de bloco.
                - var idade = 25;
            - let: Introduzido no ES6 (ECMAScript 2015), é preferível ao var. Tem escopo de bloco.
                - let nome = "João";
            - const: Também introduzido no ES6, é usado para declarar constantes, que não podem ser reatribuídas. Elas também têm escopo de bloco.
                - const PI = 3.14;
        * Tipos de Dados
            - JavaScript é uma linguagem dinamicamente tipada, o que significa que você não precisa especificar o tipo de dados ao declarar uma variável. Os tipos de dados incluem:
                - Number: Números, inteiros ou decimais.
                - String: Sequência de caracteres.
                - Boolean: Valor verdadeiro (true) ou falso (false).
                - Array: Uma coleção ordenada de valores.
                - Object: Um conjunto de pares chave-valor.
                - Null: Representa a ausência intencional de qualquer valor ou objeto.
                - Undefined: Indica que uma variável foi declarada, mas ainda não foi atribuída a um valor.
                - Symbol: Um tipo de dado cujas instâncias são únicas e imutáveis.
            - Exemplos de Uso
                - let idade = 25;
                - let nome = "João";
                - const PI = 3.14;
                - let numeros = [1, 2, 3, 4, 5];
                - let pessoa = { nome: "Maria", idade: 30 };
                - let estaChovendo = false;
                - let nulo = null;
                - let indefinido;
                - let simbolo = Symbol("chave");
        * Regras para Nomes de Variáveis
            - Os nomes de variáveis podem conter letras, dígitos, sublinhados (_) e cifrões ($).
            - O primeiro caractere não pode ser um dígito.
            - JavaScript é sensível a maiúsculas e minúsculas. nome e Nome são variáveis diferentes.
            - Não é recomendado usar palavras reservadas do JavaScript (como let, var, if, for, etc.) como nomes de variáveis.
    * Exibindo valores de variaveis para o usuário
        - Usando console.log():
            - let nome = "João";
            - let idade = 30;
            - console.log("Nome:", nome);
            - console.log("Idade:", idade);
        - Usando alert():
            - let nome = "João";
            - let idade = 30;
            - alert("Nome: " + nome + "\nIdade: " + idade);
        - Usando prompt() (para receber entrada do usuário):
            - let nome = prompt("Digite seu nome:");
            - let idade = prompt("Digite sua idade:");
            - alert("Nome: " + nome + "\nIdade: " + idade);
    * Concatenação
        - let nome = "João";
        - let sobrenome = "Silva";
        - let nomeCompleto = nome + " " + sobrenome;
        - console.log(nomeCompleto); // Saída: "João Silva"
        - console.log(`${nome} ${sobrenome}`)
    * Array básico
        - []
    * Array multidimensional
        - [ [ 2, 3 ], [ 5, 6 ] ]
    * Operadores de comparação (condicionais)
        - Igual (==): Verifica se dois valores são iguais, convertendo os tipos automaticamente, se necessário.
            - console.log(5 == 5); // Saída: true
            - console.log("5" == 5); // Saída: true (strings são convertidas para números)
        - Estritamente igual (===): Verifica se dois valores são iguais sem fazer conversão de tipo.
            - console.log(5 === 5); // Saída: true
            - console.log("5" === 5); // Saída: false (os tipos são diferentes)
        - Diferente (!=): Verifica se dois valores são diferentes, convertendo os tipos automaticamente, se necessário.
            - console.log(5 != 3); // Saída: true
            - console.log("5" != 5); // Saída: false (strings são convertidas para números)
        - Estritamente diferente (!==): Verifica se dois valores são diferentes sem fazer conversão de tipo.
            - console.log(5 !== 3); // Saída: true
            - console.log("5" !== 5); // Saída: true (os tipos são diferentes)
        - Maior que (>) e Menor que (<): Verifica se um valor é maior ou menor que outro.
            - console.log(5 > 3); // Saída: true
            - console.log(5 < 3); // Saída: false
        - Maior ou igual (>=) e Menor ou igual (<=): Verifica se um valor é maior ou igual a outro, ou menor ou igual a outro.
            - console.log(5 >= 3); // Saída: true
            - console.log(5 <= 3); // Saída: false
        - if () { }
        - else if () {}
        - else {}
    * Operadores lógicos
        - E lógico (&&): Retorna verdadeiro se ambos os operandos forem verdadeiros.
            - console.log(true && true);   // Saída: true
            - console.log(true && false);  // Saída: false
            - console.log(false && true);  // Saída: false
            - console.log(false && false); // Saída: false
        - Ou lógico (||): Retorna verdadeiro se pelo menos um dos operandos for verdadeiro.
            - console.log(true || true);   // Saída: true
            - console.log(true || false);  // Saída: true
            - console.log(false || true);  // Saída: true
            - console.log(false || false); // Saída: false
        - Negação lógica (!): Inverte o valor do operando booleano.
            - console.log(!true);  // Saída: false
            - console.log(!false); // Saída: true
        - Ternario 
            - ? & :
    * Switch
        - switch(1) {
             case 1:
                nomeDoDia = "Domingo";
                break;
            default:
                nomeDoDia = "Dia inválido";
            }
    * Operadores aritméticos
        - Adição (+): Usado para somar dois valores.
            - let resultado = 3 + 5; // resultado é 8
        - Subtração (-): Usado para subtrair o segundo valor do primeiro.
            - let resultado = 7 - 2; // resultado é 5
        - Multiplicação (*): Usado para multiplicar dois valores.
            - let resultado = 4 * 6; // resultado é 24
        - Divisão (/): Usado para dividir o primeiro valor pelo segundo.
            - let resultado = 10 / 2; // resultado é 5
        - Módulo (%): Retorna o resto da divisão do primeiro valor pelo segundo.
            - let resultado = 10 % 3; // resultado é 1
        - Potência ( ou Math.pow())**: Usado para elevar o primeiro valor à potência do segundo.
            - let resultado = 2 ** 3; // resultado é 8
    * Estrutura de repetição 
        - while
            - while (condicao) {
                // Código a ser executado enquanto a condição for verdadeira
            }
            - break
                - let i = 0;
                - while (true) {
                    console.log(i);
                    i++;
                    if (i === 10) {
                        break; // Termina o loop quando i alcança 10
                    }
                }
        - do while
            do {
                // Código a ser executado pelo menos uma vez
            } while (condicao);
        - for
            - for (inicialização; condição; expressão final) {
                // Código a ser executado em cada iteração do loop
            }
            - for (let i = 1; i <= 5; i++) {
                console.log("Contagem: " + i);
            }
    * Funções
        function nomeDaFuncao(parametro1, parametro2) {
           // Bloco de código a ser executado quando a função é chamada
        }

5 - criando o primeiro aplicativo com react native