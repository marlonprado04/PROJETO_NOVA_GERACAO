# PROJETO_CALDEIRA

Repositório com aulas, exercícios e conteúdos do Projeto Caldeira

# Índice

- [PROJETO\_CALDEIRA](#projeto_caldeira)
- [Índice](#índice)
- [Curso 4: HTML e CSS: trabalhando com responsividade e publicação de projetos](#curso-4-html-e-css-trabalhando-com-responsividade-e-publicação-de-projetos)
  - [Unidades de medidas](#unidades-de-medidas)
    - [Unidade de Medida REM](#unidade-de-medida-rem)
    - [Aplicando o REM](#aplicando-o-rem)
  - [Adaptando elementos](#adaptando-elementos)
    - [Descubra a super unidade de medida](#descubra-a-super-unidade-de-medida)
  - [Responsividade](#responsividade)
    - [Media Queries](#media-queries)
    - [Cabeçalho responsivo](#cabeçalho-responsivo)
  - [Responsividade e GitHub](#responsividade-e-github)
    - [Conteúdo responsivo](#conteúdo-responsivo)
    - [Git e GitHub](#git-e-github)
    - [Colocando o projeto no ar](#colocando-o-projeto-no-ar)
- [Aprender a lógica de programação](#aprender-a-lógica-de-programação)
  - [Comece a programar hoje](#comece-a-programar-hoje)
  - [Comunique-se com o usuário](#comunique-se-com-o-usuário)
    - [Concatenação](#concatenação)
    - [Tornando o programa dinâmico com variáveis](#tornando-o-programa-dinâmico-com-variáveis)
  - [Crie suas próprias funcionalidades](#crie-suas-próprias-funcionalidades)
    - [Melhorando a manutenção do código](#melhorando-a-manutenção-do-código)
    - [Funções](#funções)
    - [Funções com parâmetros](#funções-com-parâmetros)
  - [Pratique resolvendo problemas do seu dia a dia](#pratique-resolvendo-problemas-do-seu-dia-a-dia)
    - [Calculando o IMC](#calculando-o-imc)
    - [Retorno de funções](#retorno-de-funções)
    - [Entendendo a fundo o retorno de funções](#entendendo-a-fundo-o-retorno-de-funções)
    - [Interagindo com o usuário](#interagindo-com-o-usuário)
  - [Execute códigos diferentes dependendo da condição](#execute-códigos-diferentes-dependendo-da-condição)
    - [Convertendo texto em números](#convertendo-texto-em-números)
    - [Trabalhando com condições](#trabalhando-com-condições)
    - [Melhorando programa de IMC](#melhorando-programa-de-imc)
    - [Jogo de advinhação](#jogo-de-advinhação)
  - [Repita tarefas](#repita-tarefas)
    - [Repetir enquanto](#repetir-enquanto)
    - [Outra forma de repetir](#outra-forma-de-repetir)
    - [Acumulando valores](#acumulando-valores)
- [Links e artigos](#links-e-artigos)

# Curso 4: HTML e CSS: trabalhando com responsividade e publicação de projetos

## Unidades de medidas

### Unidade de Medida REM

O CSS permite vários tipos de medidas que são divididas em 2 grupos: medidas relativas e medidas absolutas.

As medidas interessantes de se usar são medidas relativas, pois se adaptam de acorco com as configurações do usuário.

Nesse caso vamos usar a escala de REM, que equivale a 16 pixels. Ou seja, 1 rem = 16 pixel.

### Aplicando o REM

Nessa aula vamos alterar todas as medidas de fonte que usamos pixels para rem.

## Adaptando elementos

### Descubra a super unidade de medida

Podemos usar a unidade de medida de %, porém como diz no W3SCHOOL, a % é uma unidade relativa que respeita o tamanho do "pai".

<https://www.w3schools.com/cssref/css_units.php>

## Responsividade

### Media Queries

Media queries serve para tornar o site mais responsivo e dinâmico, por exemplo, quando a imagem ocupa metade da tela sozinha em telas menores do que x pixels.

O media querie permite manipular os elementos de acordo com certas informações.

<https://developer.mozilla.org/pt-BR/docs/Web/CSS/CSS_media_queries/Using_media_queries>

Exemplo: Dentro do CSS atribuindo certos valores se a tela tiver um max-width de 1200px.

```css
@media (max-width: 1200px){
    .apresentacao{
        flex-direction: column-reverse;
    }

}
```

### Cabeçalho responsivo

Para deixar o cabeçalho responsivo, podemos adicionar um padding entre os elementos e depois centralizando o menu.

```css
... Resto do código...

    .cabecalho{
        padding: 10%; /*Atribuindo padding para separar os botões de navegação*/

    }

    .cabecalho__menu{
        justify-content: center; /*Centralizando menu de navegação*/

    }

... Resto do código...
```

## Responsividade e GitHub

### Conteúdo responsivo

Para deixar o conteúdo responsivo é necessário diminuir o **espaçamento lateral entre o conteúdo e a borda da seção completa** e depois atribuir alguma propriedade que faça a seção de conteúdo (dentro da seção completa) **consumir 100% do valor restante que não estiver sendo usado**.

Ou seja, atribuir um padding menor para o conteúdo pai e fazer o conteúdo filho consumir esse padding que foi diminuído e ficou sem uso.

Dessa forma, o código fica assim:

```css
... Restante do código...

    .apresentacao{
        flex-direction: column-reverse;
        padding: 5%; /*Diminuindo o espaçamento lateral para 5%, já que o superior e inferior já estavam esse valor, não é necessário atribuir 2 valores*/
    }

    .apresentacao__conteudo {
        width: auto; /*Atribuindo valor automático para a "seção" de apresentação de conteúdo*/

    }

... Restante do código...


```

### Git e GitHub

Link: <https://www.youtube.com/watch?v=UBAX-13g8OM>

Link do meu repositório: <https://github.com/marlonprado04/testando_git>

### Colocando o projeto no ar

Para colocar o projeot no ar podemos usar o site Vercel que permite hospedar repositórios do GitHub de forma gratuita.

OBS: Necessário que os arquivos do respositório estejam na pasta raiz para que o site funcione corretamente, ou seja, pastas com vários projetos dentro não servirão.

Link do vercel: <https://vercel.com/>

# Aprender a lógica de programação

## Comece a programar hoje

Para começar a programar é necessário ter um programa que sirva de editor para o código.

Alguns exemplos incluem o Sublime Text, Visual Studio Code ou mesmo o Notepad++.

No curso de JavaScript vamos usar o Google Chrome para interpretar o código escrito, então não é necessário um compilador ou etc (algumas linguagens necessitam disso para funcionar).

## Comunique-se com o usuário

### Concatenação

Antes de concatenar o texto do alert, foi substituido o comando alert do JavaScript pelo comando documento.write.

Para concatenar no JavaScript usamos o operador +.
A linguagem permite concatenar numeros inteiros com texto, pois ela faz a conversão do número para texto por baixo dos panos.

Sendo assim, um exemplo de código é:

```javascript

 // Concatenando
    document.write("A idade do Flávio é " + 18)

```

### Tornando o programa dinâmico com variáveis

Para declarar uma variável em JS fazemos conforme o código abaixo:

```javascript
<meta charset="UTF-8">

<script>
    var ano = 2020;

    document.write("Mário tem " + (ano - 1997) + " anos.");
    document.write("<br>");
    document.write("Marcos tem " + (ano - 1989) + " anos.");
    document.write("<br>");
    document.write("Maria tem " + (ano - 1993) + " anos.");
</script>

```

Outro exemplo de uso para poupar código:

```javascript
<meta charset="UTF-8">

<script>
    var ano = 2023;

    var idadeMario =  ano - 1997
    var idadeMarcos = ano - 1989
    var idadeMaria = ano - 1993

    var media = (idadeMarcos + idadeMaria + idadeMario)/3

    document.write("Mário tem " + idadeMario + " anos.");
    document.write("<br>");
    document.write("Marcos tem " + idadeMarcos + " anos.");
    document.write("<br>");
    document.write("Maria tem " + idadeMaria + " anos.");
    document.write("<br>");
    document.write("A média das idades é: " + Math.round(media));

</script>

```

## Crie suas próprias funcionalidades

### Melhorando a manutenção do código

Para melhorar a manutenção do código, podemos usar e abusar de recursos que as variáveis nos dão.

Por exemplo, ao invés de colocar `document.write("<br>")` para pular uma linha, podemos criar uma variável que possua essa informação.

Assim, sempre que necessário, podemos pular quantas linhas quisermos ou aumentar o número de pulos que a variável dá.

```javascript
  // Ao invés disso:

  document.write("Olá");
  document.write("<br>");
  document.write("Mundo");
  document.write("<br>");

  // Usar isso:

  var pulaLinha = "<br>";

  document.write("Olá");
  document.write(pulaLinha);
  document.write("Mundo");
  document.write(pulaLinha);
  
```

### Funções

Para declarar funções no JS o código é parecido com a criação de variáveis:

```javascript
function pulaLinha(){
  document.write("<br>");
}
```

### Funções com parâmetros

É possível criar funções que recebem parâmetros e trabalham com eles dentro da área de função.

Não é necessário criar a variável que será o passada como parâmetro para a função. Ela pode ser criada dentro da própria função, ou seja, será uma variável local dentro do escopo da função.

Exemplo:

```javascript

<meta charset="UTF-8" />

<script>
    // Criando função com parâmetro para
    // receber a mensagem quando chamada
    function mostra(mensagem){
    
        // Printando mensagem passada
        document.write(mensagem);
        // Pulando a linha
        document.write("<br>");
    }

    // Chamando a função e passando a mensagem necessária
    mostra("Olá pessoas");
</script>

```

## Pratique resolvendo problemas do seu dia a dia

### Calculando o IMC

Para calcular o IMC usando o que já foi aprendido, pode ser criada uma função que realiza a operação e aproveitar as funções anteriores para mostrar a mensagem em tela.

Dessa forma o cálculo fica dinâmico e poupa linhas de código:

```javascript
<meta charset="UTF-8" />

<script>
  // Criando função para pular linha
  function pulaLinha() {
    document.write("<br>");
    document.write("<br>");
  }

  // Criando função para printar uma mensagem
  function mostra(mensagem) {
    document.write(mensagem);
  }

  // Criando função para calcular IMC
  function calculaImc(altura, peso) {
    // Criando variável para armazenar IMC calculado
    var imc = peso / (altura * altura);

    // Printando mensagem na tela
    mostra("O IMC calculado é: " + imc);
  }

  // Executando função para calular IMC
  calculaImc(1.65, 77);
</script>

```

### Retorno de funções

Para deixar o código ainda mais dinâmico, podemos criar retorno para as funções.

Dessa forma, a função pode servir para realizar certas operações e após executar, retornar determinado valor.

Abaixo uma adaptação no código anterior incluindo essas alterações:

```javascript

  // Criando função para calcular IMC
  function calculaImc(altura, peso) {
    // Criando variável para armazenar IMC calculado
    var imc = peso / (altura * altura);

    // Retornando o IMC quando a função for chamada
    return imc;
  }

  // Criando uma variável para conter o IMC de cada pessoa
  var imcFlavio = calculaImc(1.65, 77);
  var imcMario = calculaImc(1.77, 89);

  // Mostrando o resultado atribuido em cada variável
  mostra(imcFlavio);
  mostra(imcMario);
```

### Entendendo a fundo o retorno de funções

Uma outra forma de lidar com o retorno de funções é realizar o cálculo no próprio retorno.

Por exemplo, ao invés de criar variáveis dentro da função e realizar o calculo para só então retornar o resultado do cálculo, podemos realizar todo o cálculo dentro do retorno da função.

Abaixo a adaptação do código:

```javascript

<meta charset="UTF-8" />

<script>
  // Criando função para pular linha
  function pulaLinha() {
    document.write("<br>");
    document.write("<br>");
  }

  // Criando função para printar uma mensagem
  function mostra(mensagem) {
    document.write(mensagem);
    pulaLinha();
  }

  // Criando função para calcular IMC
  function calculaImc(altura, peso) {
    // Retornando o cálculo de IMC quando a função for chamada
    return peso / (altura * altura);
  }

  // Criando uma variável para conter o IMC de cada pessoa
  var imcFlavio = calculaImc(1.65, 77);
  var imcMario = calculaImc(1.77, 89);
  var totalImc = imcFlavio + imcMario;

  // Mostrando o resultado atribuido em cada variável
  mostra(imcFlavio);
  mostra(imcMario);
  mostra(totalImc);
</script>

```

### Interagindo com o usuário

Para deixar o código ainda mais funcional e dinâmico, nós podemos coletar informações passadas pelo usuário. Para isso existe a função `prompt()` do JS.

Abaixo o código adaptado que recebe o nome, altura e peso do usuário e mostra o resultado do cálculo na tela:

```javascript
<meta charset="UTF-8" />

<script>
  // Criando função para pular linha
  function pulaLinha() {
    document.write("<br>");
    document.write("<br>");
  }

  // Criando função para printar uma mensagem
  function mostra(mensagem) {
    document.write(mensagem);
    pulaLinha();
  }

  // Criando função para calcular IMC
  function calculaImc(altura, peso) {
    // Retornando o cálculo de IMC quando a função for chamada
    return peso / (altura * altura);
  }

  // Criando uma variável para conter a altura e peso
  var nome = prompt("Informe seu nome:");
  var alturaInformada = prompt(nome + ", informe sua altura: ");
  var pesoInformado = prompt(nome + ", informe seu peso: ");
  var imc = calculaImc(alturaInformada, pesoInformado);

  // Mostrando o resultado atribuido em cada variável
  mostra(nome + ", o seu IMC é:" + imc);
</script>
```

## Execute códigos diferentes dependendo da condição

### Convertendo texto em números

A função `prompt()` do JS por padrão retorna um texto. Sendo assim, é necessário converter a informação retornada para realizar operações matemáticas.

OBS: Como o JS é uma linguagem com **variáveis dinâmicas**, as operações de **multiplicação e divisão** funcionam sem conversão, mas **ao somar os números eles acabam sendo _concatenados_**.

Para converter um valor do tipo `string` para o tipo `int` podemos usar a função padrão do JS `parseInt()` onde colocamos o valor ou variável do tipo string como parâmetro na função.

Abaixo um exemplo de código com conversão:

```javascript

<meta charset="UTF-8" />

<script>
  // Criando função para pular linha
  function pulaLinha() {
    document.write("<br>");
    document.write("<br>");
  }

  // Criando função para printar uma mensagem
  function mostra(mensagem) {
    document.write(mensagem);
    pulaLinha();
  }

  // Base do programa para calcular a pontuação de um time de futebol

  // Criando variáveis necessárias
  var vitorias = parseInt(prompt("Entre com o número de vitórias: "));
  var empates = parseInt(prompt("Entre com o número de empates: "));
  var pontos = (vitorias *3) + empates;

  // Mostrando mensagem com resultado
  mostra("Seu time tem " + pontos + " ponto(s).")
   
</script>

```

### Trabalhando com condições

Para criar condições e comparações dentro do JS usamos a função nativa `if(){}` onde passamos os parâmetros que desejamos comparar e após colocamos os cálculos desejados.

Exemplo:

```javascript

<meta charset="UTF-8" />

<script>
  // Criando função para pular linha
  function pulaLinha() {
    document.write("<br>");
    document.write("<br>");
  }

  // Criando função para printar uma mensagem
  function mostra(mensagem) {
    document.write(mensagem);
    pulaLinha();
  }

  // Base do programa para calcular a pontuação de um time de futebol

  // Criando variáveis necessárias
  var vitorias = parseInt(prompt("Entre com o número de vitórias: "));
  var empates = parseInt(prompt("Entre com o número de empates: "));
  var pontos = vitorias * 3 + empates;

  // Mostrando mensagem com resultado
  mostra("Seu time tem " + pontos + " ponto(s).");


  // Criando condições para mensagem
  if (pontos > 28) {
    mostra("Seu time está MELHOR que ano passado.");
  }

  if (pontos < 28) {
    mostra("Seu time está PIOR que ano passado.");
  }
  if (pontos == 28) {
    mostra("Seu time está IGUAL ao ano passado.");
  }
</script>

```

### Melhorando programa de IMC

Para deixar o programa de cálculo de IMC criado anteriormente mais funcional, vamos incluir o conteúdo aprendido até então.

Abaixo o código alterado:

```javascript
<meta charset="UTF-8" />

<script>
  // Criando função para pular linha
  function pulaLinha() {
    document.write("<br>");
    document.write("<br>");
  }

  // Criando função para printar uma mensagem
  function mostra(mensagem) {
    document.write(mensagem);
    pulaLinha();
  }

  // Criando função para calcular IMC
  function calculaImc(altura, peso) {
    // Retornando o cálculo de IMC quando a função for chamada
    return peso / (altura * altura);
  }

  // Criando uma variável para conter a altura e peso
  var nome = prompt("Informe seu nome:");
  var alturaInformada = prompt(nome + ", informe sua altura: ");
  var pesoInformado = prompt(nome + ", informe seu peso: ");
  var imc = calculaImc(alturaInformada, pesoInformado);

  // Mostrando o resultado atribuido em cada variável
  mostra(nome + ", o seu IMC é:" + imc);

  // Criando operador para comparar IMC do usuário com o ideal
  if (imc < 18.5) {
    mostra("Seu IMC está ABAIXO do recomendado!");
  }

  if (imc > 35) {
    mostra("Seu IMC está ACIMA do recomendado!");
  }

  if (imc >= 18.5 && imc <= 35) {
    mostra("Seu IMC está EXCELENTE!");
  }
</script>
```

### Jogo de advinhação

Com tudo aprendido até aqui podemos criar um jogo de adivinhação, conforme código abaixo:

```javascript

<meta charset="UTF-8" />

<script>
  // Criando função para pular linha
  function pulaLinha() {
    document.write("<br>");
    document.write("<br>");
  }

  // Criando função para printar uma mensagem
  function mostra(mensagem) {
    document.write(mensagem);
    pulaLinha();
  }

  // Criando variável que recebe um número aleatório gerado a partir das funções round() e random() da biblioteca Math
  var numeroPensado = Math.round(Math.random() * 10);

  // Criando variável para receber chute do usuário
  var chute = parseInt(prompt("Digite um chute: "));

  // Comparando chute com o número gerado
  if (chute == numeroPensado) {
    mostra("Você acertou!");
  } else {
    mostra("Você errou, o número pensado foi " + numeroPensado);
  }
</script>

```

> Desafio:
>1 - Você pode criar uma função sorteia que recebe um número n e sorteia um número entre 0 a n, retornando esse valor. Dessa forma, em vez de escrever var numeroPensado = Math.round(Math.random() * n);, você escreveria var numeroPensado = sorteia(n);. Faça essa modificação, criando a nova função e utilize-a.

```javascript
<meta charset="UTF-8" />

<script>
  // Criando função para pular linha
  function pulaLinha() {
    document.write("<br>");
    document.write("<br>");
  }

  // Criando função para printar uma mensagem
  function mostra(mensagem) {
    document.write(mensagem);
    pulaLinha();
  }

  // Criano função para sortear número
  function sorteia(n){
    // Retornando número de acordo com sugestão do usuário
    return Math.round(Math.random() * n);
  }

  // Criando variável para receber o número máximo de sorteio sugerido pelo usuário
  var numeroMaximo = parseInt(prompt("Digite até que número deseja o sorteio: "));

  // Criando variável de número sorteado
  var numeroSorteado = sorteia(numeroMaximo);

  // Criando variável para receber chute do usuário
  var chute = parseInt(prompt("Digite um chute: "));
  
  // Comparando chute com o número gerado
  if (chute == numeroSorteado) {
    mostra("Você acertou!");
  } else {
    mostra("Você errou, o número pensado foi " + numeroSorteado);
  }
</script>

```

## Repita tarefas

### Repetir enquanto

Para repetir operações podemos usar o laço de repetição `while(){}`. Nele atribuimos uma condição e enquanto ela estiver sendo `true`, o código dentro dela permanece sendo executado.

Abaixo um programa que lista todos os anos em que houveram copa adicionando + 4 a cada ano, de acordo com data limite que o usuário estipular:

```javascript
<meta charset="UTF-8" />

<script>
  // Criando função para pular linha
  function pulaLinha() {
    document.write("<br>");
    document.write("<br>");
  }

  // Criando função para printar uma mensagem
  function mostra(mensagem) {
    document.write(mensagem);
    pulaLinha();
  }

  // Programa para calcular o ano em que haverá copa

  // Declarando variáveis
  var anoCopa = 1930;
  var dataLimite = parseInt(prompt("Digite a data limite: "));

  // Criando laço de repetição para gerar alerta informando anos que houveram copa
  while(anoCopa <= dataLimite){
    mostra("Teve copa em " + anoCopa);
    anoCopa = anoCopa+4;
  }

  mostra("FIM");
 
</script>
```

### Outra forma de repetir

Uma alternativa ao `while` é o `for`, que funciona da mesma forma, porém não é necessário criar variáveis antes da excução.

Abaixo um código que calcula a tabuada:

```javascript
<meta charset="UTF-8" />

<script>
  // Criando função para pular linha
  function pulaLinha() {
    document.write("<br>");
    document.write("<br>");
  }

  // Criando função para printar uma mensagem
  function mostra(mensagem) {
    document.write(mensagem);
    pulaLinha();
  }

  // Programa para calcular tabuada

  // Criando laço de repetição com for

  for (var multiplicador = 1; multiplicador <= 10; multiplicador++) {

    mostra("7*" + multiplicador + "=" + (7*multiplicador));
  }
</script>

```

### Acumulando valores

Podemos usar os laços de repetição para acumular valores e realizar operações de acordo.

Por exemplo, perguntar para o usuário um numero de pessoas que ele deseja calcular a média de idades e criar um laço para pedir todas as idades e depois realizar o calculo da média.

Abaixo o código de exemplo:

```javascript
<meta charset="UTF-8" />

<script>
  // Criando função para pular linha
  function pulaLinha() {
    document.write("<br>");
    document.write("<br>");
  }

  // Criando função para printar uma mensagem
  function mostra(mensagem) {
    document.write(mensagem);
    pulaLinha();
  }

  // Progrma para calcular a média das idades de acordo com o número de pessoas informado pelo usuário

  // Criando variáveis
  var totalPessoas = parseInt(prompt("Quantas pessoas? "));
  var numero = 1;
  var totalIdades = 0;
  var mediaDasIdades = 0;

  // Criando laço de repetição
  while(numero <= totalPessoas){
    var idade = parseInt(prompt("Informe a idade: "));
    totalIdades = totalIdades + idade;
    numero ++;
  }

  // Atribuindo cálculo de média das idades à variável
  mediaDasIdades = totalIdades / totalPessoas;

  // Mostrando mensagem na tela
  mostra("A média das idades é: " + mediaDasIdades);

</script>

```

# Links e artigos

Guia da Alura de unidades no CSS: <https://www.alura.com.br/artigos/guia-de-unidades-no-css>

Podcast Alura: <https://cursos.alura.com.br/extra/hipsterstech/css-cansei-de-ser-simples-hipsters-09-a577>

5 dúvidas de quem quer começar com TI: <https://www.alura.com.br/artigos/5-duvidas-de-quem-quer-iniciar-na-carreira-de-programacao>
