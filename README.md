<picture>
  <source media='(prefers-color-scheme: dark)' srcset='./public/github-images/banner-dark.png'>
  <img src='./public/github-images/banner-light.png' alt=''>
</picture>

<h1 align='center'>Putting the "You" in CPU (tradução)</h1>
<!-- <p align='center'>A technical explainer of how your computer runs programs, from start to finish.</p> -->
<p align='center'> Uma explicação técnia de como seu computador executa programas, do início ao fim </p>
<p align='center'> por <a href='https://github.com/kognise'>@kognise</a> e <a href='https://github.com/hackclub'>@hackclub</a></p>
<p align='center'> Tradução em andamento por <a href='https://github.com/lucasoshiro'>@lucasoshiro</a></p>
<br>

<!-- ## From the beginning... -->

## Do começo

**Nota de tradução:** _Esta é uma tradução de [https://cpu.land](https://cpu.land), que achei excelente pela forma simples de abordar um assunto tão complexo. Traduzir para português é uma forma de ajudar a disseminar ainda mais o que foi feito originalmente como uma forma de retribuição. Tudo daqui para a frente é de autoria de [Lexi Mattick](https://kognise.dev/), que além de ter escrito e disponibilizado gratuitamente, ainda o publicou sobre a licença MIT, que permite a redistribuição e reuso do que foi feito. Todo o mérito do próximo parágrafo em diante é dela, e se você gostar do que leu, peço que deixe uma estrela no [repositório original do GitHub](https://github.com/hackclub/putting-the-you-in-cpu/tree/main), como forma de agradecimento e também para incentivar iniciativas como estas. Alguns termos mantive o nome original em inglês dentro de parênteses para facilitar o estudo de quem for ler. O texto original é escrito de forma bem informal e várias expressões não têm equivalentes em português, mas tentei fazer o possível para manter fiel em relação ao texto original da Lexi, já que isso é parte do que o torna tão bom._

<!-- I’ve done a lot of things with computers, but I’ve always had a gap in my knowledge: what exactly happens when you run a program on your computer? I thought about this gap — I had most of the requisite low-level knowledge, but I was struggling to piece everything together. Are programs really executing directly on the CPU, or is something else going on? I’ve used syscalls, but how do they work? What are they, really? How do multiple programs run at the same time? -->

Eu já fiz [várias coisas com computadores](https://github.com/kognise), mas sempre tive uma lacuna em meu conhecimento: o que exatamente acontece quando você executa um programa em seu computador? Eu pensei sobre essa lacuna - Eu tinha a maior parte do conhecimento de baixo nível, mas eu estava com dificuldade de juntar tudo. Os programas são realmente executados diretamente na CPU, ou existe alguma outra coisa acontecendo? Eu já usei syscalls, mas como elas realmente *funcionam*? O que são elas, de verdade? Como múltiplos programas são executados ao mesmo tempo?

<!-- <img src='/images/writing-this-article.png' loading='eager' style='margin: 40px 0;' alt='A scrawled digital drawing. Someone with long hair is confused as they peer down at a computer ingesting binary. Suddenly, they have an idea! They start researching on a desktop computer with bad posture.' width='1708' height='536' /> -->

<img src='public/images/writing-this-article.png' loading='eager' style='margin: 40px 0;' alt='Um esboço digital. Uma pessoa com cabelo comprido está confusa enquanto olha para baixo para um computador recebendo um binário. Do nada, tem uma ideia! Começa a pesquisar em um computador desktop em uma má póstura.' width='700'/>

<!-- I cracked and started figuring as much out as possible. There aren't many comprehensive systems resources if you aren't going to college, so I had to sift through tons of different sources of varying quality and sometimes conflicting information. A couple weeks of research and almost 40 pages of notes later, I think I have a much better idea of how computers work from startup to program execution. I would've killed for one solid article explaining what I learned, so I'm writing the article that I wished I had. -->

Eu fucei e comecei a descobrir o máximo que pude. Não existem muitos recursos compreensíveis se você não vai para a faculdade, então tive que peneirar entre várias diferentes fontes de qualidades variadas e às vezes com informações conflituosas. Algumas semanas de pesquisa e quase 40 páginas de notas depois, eu acho que tenho uma ideia bem melhor de como computadores funcionam desde quando ligam até a execução de programas. Eu realmente gostaria que tivesse um artigo sólido explicando o que aprendi, então estou escrevendo o artigo que eu gostaria que tivesse.

<!-- And you know what they say... you only truly understand something if you can explain it to someone else. -->

E você sabe o que dizem... você só consegue entender algo de verdade se você conseguir explicar para alguém.

<!-- > In a hurry? Feel like you know this stuff already? -->
> Com pressa? Sente que já sabe isso?
>
<!-- > [Read chapter 3](/how-to-run-a-program) and I guarantee you will learn something new. Unless you're like, Linus Torvalds himself. -->

> [Leia o capítulo 3](https://cpu.land/how-to-run-a-program) e eu garanto que você vai aprender algo novo. A não ser que você seja, sei lá, Linus Torvalds.

<br>

<!-- <p align='center'><a href='https://cpu.land/the-basics'><strong>Continue to Chapter 1: The "Basics" &raquo;</strong><br>(cpu.land)</a></p> -->
<p align='center'><a href='https://cpu.land/the-basics'><strong>Continue no capítulo 11: O "Básico" &raquo;</strong><br>(cpu.land)</a></p>
