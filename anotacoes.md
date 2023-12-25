# Notion: https://humane-legend-9f9.notion.site/Workshop-como-iniciar-um-projeto-sem-travar-Passo-Passo-ba62ca9812f445838e4db7a1a19bfdcb


## Dividimos a construção de qualquer software nas seguintes etapas:

1. análise
    a. análise do projeto(Vai dar uma olhada no projeto e analisar o que ele tem. No Front-End Mentor não tem acesso ao figma, então preciso analisar o que tem no projeto.)

    b. anotar as dúvidas e vai tirar as dúvidas com o designer
    (Mas toma cuidado para não perguntar tudo. Você no começo tem que saber se virar um pouco. Perguntar sobre mais assuntos complexos. Em uma empresa fica um pouco mais complicado, precisa se virar como um programador iniciante.
    E depois, olhar as telas, abrir o projeto, olhar páginas, vai analisar por cima o que precisamos construir exatamente.)

    c. olhar as telas e tentar componentizar
    (Tentar quebrar a página em componentes. As vezes estamos fazendo um site que tem mais de uma página. Tem 5, 10, 20 páginas e elas tem coisas em comum. Botões por exemplo. Componentes são pequenos pedacinhos do site que as vezes podemos reaproveitar e usar em outros lugares e é melhor você fazer separado para poder reaproveitar e ganhar tempo. Para que fazer algo na mão sendo que dá para aproveitar? Isso é falta de analise. E já criando os componentes... O que posso criar para poder reutilizar? Isso acelera o desenvolvimento e melhora a manutenção. Alguns projetos não precisam fazer isso, e tá tudo bem.)

    d. pensar na estrutura base
    (O que preciso construir? Como construir? Div, section... Tudo isso já pode começar a pensar. Até dá para desenhar como vai ficar o meu projeto, a base dele pelo menos. 
    Se você pensar em blocos fica mais fácil.)


2. criar a estrutura base do projeto
    a. criar estrutura de pastas
    (Criar a pasta src e dentro da pasta vai colocar as pastas css, img, js e depois vai colocar os arquivos dentro dela. E vai criar depois o index.html dentro da pasta raiz. Estrutura padrão. Os projetos mais simples vai ser dessa maneira. É diferente do que fazer um projeto react.)

3. Criar o html
    1. criar o index.html
    (Sempre criar o principal arquivo HTML com o nome de index. Sites de servidores de web, não vão conseguir carregar sem ter esse nome.)

    2. criar a estrutura base do html(Geralmente começamos criando as sessões ou divs maiores e aos poucos vamos entrando em cada uma delas e criando as tags e os elementos HTMl dentro delas.
    Nunca se preocupe em criar o HTML perfeito. Isso nunca vai existir!)
    
4. criar o CSS
    1. criar o arquivo de reset.css
    (Em casos de projetos um pouco mais complexos, criar esse arquivo.)
    2. criar o arquivo de estilos, estilo.css
    (Começar a estilizar o site nesse arquivo. Estilize de cima para baixo. Começando pelo menu chegando até o rodapé. Sempre de cima para baixo e da esquerda para a direita, igual a leitura. Comece estilizando a base e depois estilizando os itens, as sessões as divs de dentro.
    Tome cuidado para não estilizar um menu difícil e querer estilizar o rodapé primeiro.)

5. criar o JS
    1. se tiver
    2. primeiro pensar na lógica pra depois ir para o código(Nada de sair fazendo código sem pensar no que está fazendo.)


`Refatorar` -> Fazer o código funcionar primeiro e depois deixar o código mais limpo. Sem adicionar novas funcionalidades. Apenas aplicar conteúdos de clean code.

*E se eu travar na hora de começar meu projeto?* -> É normal travar. Quando você trava é porque tem alguma dúvida de como prosseguir. O melhor jeito é perguntar. Tire as dúvidas. No discord tirar as dúvidas que eles vão dar um encaminhamento.

`Pasta design` -> Essa pasta mostra como vai ficar o projeto em cada modelo, seja desktop ou mobile. No arquivo `active-states.jpg` prestar atenção, porque é um arquivo que contém tarefas de cursor(hover css).

`style-guide.md` -> Este arquivo mostra tudo o que temos que usar no projeto. 

Na parte layout, é sempre fazer todas as resoluções responsivas. Tem que fazer na resolução 768 do iPad. A menos que o design pede para fazer nas resoluções que ele queira.

Quando você estiver em uma empresa que trabalha com Front-End, provavelmente terá um arquivo style-guide.

`README.md` -> Dá informações sobre o que é o desafio, como fazer, o que tem nele...
Dá algumas informações sobre o projeto. 
Se não sei inglês, colocar no google tradutor.

`README-template.md` -> Usar para se basear no projeto que você fez. Na hora que for colocar o seu projeto no github, utilizar esse arquivo.
Não é bom deixar o template que vem junto com o Front-End Mentor, não é bom deixar como ele está. Faça seu próprio README.md 

## Começar a fazer o projeto 37:53

46:44(PRESTAR ATENÇÃO NESSA PARTE!!!) ->  Agora vamos começar a criar a estrutura dentro do body. Agora é a parte que precisamos começar a pensar. Como iremos criar a estrutura HTML de acordo com o projeto?
Analisar é um dos fatores que fazem não tratar. Analise o design.

Aprenda pelo menos display: flex para fazer os projetos de HTML e CSS.

![img/img1.png](/src/images/img1.png)

Tudo o que é principal na página vai dentro da tag `main`.

Errou? Conserta! Você nunca vai acertar nada de primeira.

Fazer as classes quando for fazer o CSS.

Pode ser que você termine de montar o seu HTML, mas terá que mudar ele futuramente. E isso é completamente normal. Não existe o HTML perfeito!

## 1:07:51 Fazendo o CSS

Se não tenho o figma, como que faço para olhar a largura e a altura do componente?
Irei baixar a extensão Perfect Pixel para instalar no browser que utilizo.
Com essa extensão dá para ter uma noção de fonte, de margin, de padding, de largura...

Background-color ou border são o console.log do CSS. Como assim?
É uma forma da gente debugar/entender o que está acontecendo com o código. Saber o que é aquele elemento, o tamanho que ele está ocupando.

Aonde dar um display: flex? Poderia ser no body? Até poderia. Só que ele vai alinhar horizontalmente.
Então iremos fazer no main. E no body, geralmente, não é bom ficar estilizando um monte de coisa nele.

Vamos prestar atenção nisso:

```css
main {
  display: flex;
  justify-content: center;
  align-items: center; /* Sem uma altura definida, essa propriedade não vai funcionar. Sempre colocar uma altura de 100vh.*/
}
```

Sempre cria classes no HTML. Fica mais específico e mais fácil também de entender o código.


Em cada conteúdo que você for fazer, faças as classes na hora. Não faça as classes tudo de uma vez para depois estilizar no CSS.

## Actives 2:13:10

Acessando a pasta design e clicar no arquivo active-states, podemos ver a parte do que temos que fazer no active.

Na parte da imagem, teremos que colocar um overlay na imagem e uma imagem dentro que é o olho.

![active states](../design/active-states.jpg)

A maneira mais fácil de fazer isso é usando before e after. Podemos criar um pseudo-elemento para essa div azul e um pseudo-elemento para o olho.

Prestar atenção -> 2:22:31 -> Neste tempo ele vai estar explicando sobre o before que usamos no
.image-link.

```css
.nft-card .image-link {
  position: relative; /* Sempre colocar position: relative no pai */
  display: flex;
  /* Dá onde o image-link está pegando essa largura e altura de 300px se não definimos nada aqui? 
  A largura e a altura vem da imagem(.image) */
}

.nft-card .image-link::before {
  content: '';
  background-color: cyan;
  width: 100%;
  height: 100%;
  position: absolute; /* Usamos position: absolute para posicionar o elemento por cima da imagem. Iremos ter o fundo e aquele olho que são duas coisas separadas. Então teremos que usar o position: absolute para posicionar tanto o esse fundo, quanto o olho também depois. 
  Quando tiramos o position: absolute, no elemento before é como se ele estivesse escondido depois da imagem. Quando colocamos o position: absolute ele sai do contexto padrão do browser. E com o position: absolute, conseguimos setar 100% da largura e altura do .image-link(pai). E a ideia é usar o position: relative no pai do elemento. Se não lembra, rever a aula de position: absolute no CSS intermediário. */
  opacity: 0.4;
}
```

Estude mais sobre o conceito de before e after

## Responsivo 2:35:48

Verificar se tem a extensão Responsive View. Se não tiver, baixa.

Nem é necessário criar um responsivo

## Fim do projeto 2:38:08 

O que fica com o projeto?

Na hora de fazer um projeto do Front-End Mentor, use o workshop para fazer outros projetos.

**Sempre analise os assuntos do projeto antes de começar a codar. Isso vai evitar travar mais.**
Até o cadu e o beto travaram na hora de fazer os positions... E isso vai acontecer naturalmente.
Programadores sêniors vão travar também, vão pedir ajudar também e não são robôs para saberem de tudo.

Quanto mais você praticar, mais você vai ficar maduro e vai destravar mais rápido.
A mentalidade de agora é analisar antes as coisas antes de começar a codar. Comece daqui para frente.

No CSS tem algumas coisas que precisam ser refatoradas. Coloque o projeto no github e refatore depois.

