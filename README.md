# Git
![NPM](https://img.shields.io/npm/l/react)
# Introdução

O sistema de controle de versão moderno mais usado no mundo hoje é o Git. O Git é um projeto de código aberto maduro e com manutenção ativa desenvolvido em 2005 por [Linus Torvalds](#), o famoso criador do kernel do sistema operacional Linux. Um número impressionante de projetos de software depende do Git para controle de versão, incluindo projetos comerciais e de código-fonte aberto. Os desenvolvedores que trabalharam com o Git estão bem representados no pool de talentos de desenvolvimento de software disponíveis e funcionam bem em uma ampla variedade de sistemas operacionais e IDEs (Ambientes de Desenvolvimento Integrado).

Tendo uma arquitetura distribuída, o Git é um exemplo de [DVCS](#) (Sistema de Controle de Versão Distribuído). Em vez de ter apenas um único local para o histórico completo da versão do software, como é comum em sistemas de controle de versão como o [CVS](#) ou [SVN](#), no Git, a cópia de trabalho de todo desenvolvedor do código também é um repositório que pode conter o histórico completo de todas as alterações. Além de ser distribuído, o Git foi projetado com desempenho, segurança e flexibilidade em mente.

**Desempenho**

As características brutas de desempenho do Git são muito fortes quando comparadas a muitas alternativas. Fazer o commit de novas alterações, branches, mesclagem e comparação de versões anteriores – tudo é otimizado para desempenho. Os algoritmos implementados no Git aproveitam o conhecimento profundo sobre atributos comuns de árvores de arquivos de código-fonte reais, como costumam ser modificados ao longo do tempo e quais são os padrões de acesso.

Diferente de alguns softwares de controle de versão, o Git não se deixa enganar pelos nomes dos arquivos ao determinar qual deve ser o armazenamento e o histórico de versões da árvore de arquivos. Em vez disso, o Git se concentra no conteúdo do arquivo. Afinal, os arquivos de código-fonte são renomeados, divididos e reorganizados com frequência. O formato do objeto dos arquivos de repositório do Git usa uma combinação de codificação delta (armazenamento de diferenças de conteúdo) e compactação e armazena com clareza o conteúdo do diretório e os objetos de metadados da versão.

A distribuição também oferece benefícios significativos de desempenho.

Por exemplo, digamos que uma desenvolvedora, Alice, faça alterações no código-fonte, adicionando um recurso para a próxima versão, 2.0, e faça o commit dessas alterações com mensagens descritivas. Ela então trabalha em um segundo recurso e faz o commit dessas alterações também. Como esperado, eles são armazenados como peças de trabalho separadas no histórico de versões. Alice então muda para o branch da versão 1.3 do mesmo software para corrigir um erro que afeta apenas a versão mais antiga. O objetivo disso é permitir que a equipe de Alice lance uma versão de correção de bug, a versão 1.3.1, antes que a versão 2.0 esteja pronta. Alice pode retornar ao branch 2.0 para continuar trabalhando nos novos recursos da versão 2.0. Tudo isso pode ocorrer sem nenhum acesso à rede e, portanto, é um processo rápido e confiável. Ela poderia até fazer isso em um avião. Quando estiver pronta para fazer o commit de todas as alterações como itens individuais no repositório remoto, Alice vai poder enviar todas elas por push em um único comando.

Segurança
O Git foi projetado com a integridade do código-fonte gerenciado como uma prioridade. O conteúdo dos arquivos, bem como os verdadeiros relacionamentos entre arquivos e diretórios, versões, tags e commits, todos esses objetos no repositório do Git são protegidos com um algoritmo de hash de criptografia seguro chamado SHA1. Isso protege o código e o histórico de alterações contra alterações acidentais e maliciosas e garante que o histórico tenha rastreabilidade total.

Com o Git, você pode ter certeza de ter um histórico de conteúdo autêntico do código-fonte.

Alguns outros sistemas de controle de versão não têm proteções contra alterações secretas posteriores. Isso pode ser uma vulnerabilidade séria de segurança das informações para qualquer empresa que depende do desenvolvimento de software.

Flexibilidade
Um dos principais objetivos de design do Git é a flexibilidade. O Git é flexível em vários aspectos: suporte a vários tipos de fluxos de trabalho de desenvolvimento não lineares, em eficiência em projetos pequenos e grandes e em compatibilidade com muitos sistemas e protocolos existentes.

O Git foi projetado para tratar os branches e tags como cidadãos de primeira classe (ao contrário do SVN) e operações que afetam branches e tags (como mesclagem ou reversão) também são armazenadas como parte do histórico de alterações. Nem todos os sistemas de controle de versão apresentam esse nível de rastreamento.

Controle de versões com Git
Hoje, o Git é a melhor escolha para a maioria das equipes de software. Embora cada equipe seja diferente e deva fazer a própria análise, aqui estão os principais motivos pelos quais o controle de versão com Git é preferido em vez de alternativas:

O Git é bom
O Git tem a funcionalidade, desempenho, segurança e flexibilidade que a maioria das equipes e desenvolvedores individuais precisa. Esses atributos do Git são explicados acima. Nas comparações lado a lado com a maioria das outras alternativas, muitas equipes acham que o Git é muito favorável.

Git é um padrão de fato
O Git é a ferramenta mais adotada da categoria. Ele é atraente pelos seguintes motivos. Na Atlassian, quase todo código-fonte do projeto é gerenciado no Git.

Um grande número de desenvolvedores já tem experiência com o Git e uma proporção significativa de recém-formados pode ter experiência apenas com o Git. Embora algumas empresas precisem escalar a curva de aprendizado ao migrar para o Git de outro sistema de controle de versão, muitos desenvolvedores existentes e futuros não precisam ser treinados no Git.

Além dos benefícios de um grande conjunto de talentos, a predominância do Git também significa que muitas ferramentas e serviços de software de terceiros já estão integrados ao Git, incluindo IDEs e novas ferramentas de uso como o cliente de desktop DVCS Sourcetree, software de rastreamento de itens e projetos, Jira, e serviço de hospedagem de código, Bitbucket.

Se você é um desenvolvedor inexperiente que quer desenvolver habilidades valiosas em ferramentas de desenvolvimento de software, quando se trata de controle de versão, o Git deve ser um dos itens na lista.

Git é um projeto de código aberto de qualidade
O Git é um projeto de código aberto muito bem suportado, com mais de uma década de administração sólida. Os mantenedores do projeto mostraram um julgamento equilibrado e uma abordagem madura para atender às necessidades de longo prazo dos usuários, com lançamentos regulares que melhoram a usabilidade e a funcionalidade. É fácil examinar a qualidade do software de código aberto, e inúmeras empresas dependem muito dessa qualidade.

O Git tem excelente suporte da comunidade e uma vasta base de usuários. A documentação é excelente e abundante, incluindo livros, tutoriais e sites dedicados. Existem também podcasts e tutoriais em vídeo.

O código aberto reduz o custo para desenvolvedores amadores, pois eles podem usar o Git sem pagar uma taxa. Para uso em projetos de código aberto, o Git é sem dúvida o sucessor das gerações anteriores de sistemas bem-sucedidos de controle de versão de código aberto, SVN e CVS.

Crítica ao Git
Uma crítica comum ao Git é que pode ser difícil de aprender. Algumas das terminologias do Git vão ser novas para os iniciantes e, para usuários de outros sistemas, a terminologia do Git pode ser diferente, por exemplo, revert no Git tem um significado diferente do que no SVN ou CVS. No entanto, o Git é muito capaz e disponibiliza muitos recursos aos usuários. Aprender a usar esses recursos pode levar algum tempo. No entanto, uma vez aprendidos, podem ser usados pela equipe para aumentar a velocidade de desenvolvimento.

Para as equipes que vêm de um VCS não distribuído, ter um repositório central pode parecer uma coisa boa que eles não querem perder. No entanto, embora o Git tenha sido projetado como um sistema de controle de versão distribuído (DVCS), com o Git, você ainda pode ter um repositório canônico oficial em que todas as alterações no software devem ser armazenadas. Com o Git, como o repositório de cada desenvolvedor está completo, o trabalho não precisa ser restringido pela disponibilidade e desempenho do servidor "central". Durante interrupções ou quando offline, os desenvolvedores ainda podem consultar o histórico completo do projeto. Como o Git é flexível e está sendo distribuído, você pode trabalhar da maneira que está acostumado, mas obter os benefícios adicionais do Git, alguns dos quais você nem percebe que está perdendo.

Agora que você entende o que é o controle de versão, o que é o Git e por que as equipes de software deveriam optar por ele, continue lendo para descobrir os benefícios que o Git pode oferecer em toda a empresa.

```bash
#01) Baixe e instale o VSC e depois o Git (escolha o VSC como Git padrão).
#02) Instale o plugin "Git Graph" no VSC.
#03) Você pode usar o MSDos, o Git Bash ou o Terminal do VSC.
#04) Teste o comando "git version".
git version

#05) É preciso definir um "Usuário" e "E-mail" padrão no Git.
git config --global user.name "Fred"

#06) Digite: git config --global user.name "Fred" (utilize: git config user.name, para checar).
git config user.name

#07) Digite: git config --global user.email "fred@fred.com" (utilize: git config user.email, para checar).
git config --global user.email "fred@fred.com"

#utilize: git config user.email, para checar
git config user.email
```

Existem programas profissionais para criação de páginas em HTML, como o Visual Studio Code ou Notepad++. Apesar da enorme importância para o mundo da informação, o HTML estancou na versão 4.0.1 desde 1999 e não acompanhou as dinâmicas mudanças que ocorreram nos últimos anos e para atender as necessidades careceu utilizar plugins externos como o já aposentado [Adobe Flash Player](https://pt.wikipedia.org/wiki/Adobe_Flash_Player) e outros. Mas felizmente, isso são coisas do passado, pois a [W3C](https://pt.wikipedia.org/wiki/W3C) (World Wide Web Consortium) e a [WHATWG](https://pt.wikipedia.org/wiki/WHATWG) (Web Hypertext Application Technology Working Group) disponibilizaram a versão HTML 5.

## O que é o HTML5

O HTML5 é o novo padrão para a estruturação e apresentação de conteúdo na Word Wide Web trazendo melhorias significativas com novas funcionalidades de semântica e acessibilidade, além de melhorar o suporte aos mais recentes conteúdo multimídias. As principais mudanças que a nova versão proporciona aos usuários são: 

- Melhor tratamento de exceção
- Mais tags para substituir scripts
- Independência de plataforma 
- Redução da necessidade de plugins externos.

## As características do HTML5

As características da versão 5 estão ligadas diretamente as necessidades de suporte independente aos novos formatos de conteúdo multimídia, as novas funcionalidades de semânticas e acessibilidade. Na sequência destacamos suas principais características:

**a) Inclusão do elemento Canvas para desenho.**

O elemento Canvas foi incluído para permitir desenhar gráficos em uma página Web, tarefa essa que atualmente só é possível com a utilização de plugins externos. Neste curso não trabalharemos com o elemento Canvas.

**b) Inclusão dos elementos vídeo e áudio para reprodução multimídia**

Outro motivo para integrar plugins externos é o uso de áudio e vídeo nas páginas Web. Com a inclusão de tags específicas para este fim, o HTML5 dá suporte nativo para a reprodução de áudio e vídeo, sem a necessidade de utilizar mecanismos externos. 

```html
<!-- Exemplo de faixa de áudio -->
	<audio controls>
		<source src="horse.mp3" type="audio/mpeg">
	</audio>
	<br><br>
	<!-- Exemplo de faixa de vídeo e legenda -->
	<video width="320" height="240" controls>
		<source src="forrest_gump.mp4" type="video/mp4">
		<track src="fgsubtitles_en.vtt" kind="subtitles" srclang="en" label="English">
	</video>
```

**c) Melhor suporte para armazenamento local**

Inclusão de novos objetos para armazenamento de dados locais. Estes procedimentos não serão abordados neste curso, uma vez que a manipulação de arquivos depende do uso de uma outra linguagem no [back-end](https://pt.wikipedia.org/wiki/Front-end_e_back-end).

**d) Inclusão de novos elementos de conteúdo específico.**

Muitos elementos da versão 4.0.1 foram excluídos da nova versão, uns por nunca terem sido usados, outros por estarem obsoletos e outros por serem usados indevidamente. A versão 5 traz novos elementos para proporcionar aos usuários uma melhor estrutura, desenho e conteúdo multimídia (denominados elementos semânticos). A relação completa desses elementos será abordada durante o curso, mas abaixo segue uma prévia:

```html
<!-- Exemplo de elementos semânticos -->
	<section class="section-1">
            <article class="div-3-left">
                <header>
                    <h1>Lorem ipsum dolor sit amet consectetur.</h1>
                </header>
                <section>
                    <img src="https://picsum.photos/id/816/350/200" class="img-highlight">
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. 
                    <a href="#" class="a-link">Continuar</a>
                </section>
            </article>
    </section>
```

**e) Inclusão de novos controles para formulário.**

Uma carência da versão 4.0.1 é a escassa quantidade de controles para formulário, fazendo com que os desenvolvedores recorram as famosas bibliotecas JavaScript, muitas vezes incompatíveis com determinados navegadores. Na versão 5 novos controles de formulário foram incluídos para facilitar a vida dos desenvolvedores. Um dos remanescentes da versão 4.0.1, o elemento input, ganhou novos valores para o atributo type, fazendo com que o desenvolvedor ganhe maior controle sobre a entrada de dados pelo usuário. Abaixo, uma prévia desses itens:

```html
<!-- Entrada do tipo cor -->
    <label>Cores</label><br>
    <input type="color"><br><br>

<!-- Entrada do tipo data -->
    <label>Data</label><br>
    <input type="date"><br><br>

<!-- Entrada do tipo mês -->
    <label>Mês</label><br>
    <input type="month"><br><br>

<!-- Entrada do tipo semana -->
    <label>Semana</label><br>
    <input type="week">
```

**f) Total suporte ao CSS3**

Para dar ainda mais liberdade à criatividade dos usuários, o HTML5 dá total suporte a mais nova versão das famosas Cascading Style Sheets, ou simplesmente CSS. Com essa integração, as páginas Web podem receber os mais variados tipos de estilos como sombra nos textos e quadros, efeitos de transição, quadro com cantos arredondados e vários recursos que o CSS3 oferece.

No vídeo abaixo da Dotec, é apresentado um pequeno resumo do que é o HTML e sua aplicabilidade. 

[![Assista ao vídeo](https://img.youtube.com/vi/Tld2CrT5c2s/maxresdefault.jpg)](https://www.youtube.com/watch?v=Tld2CrT5c2s)

## Referências

- https://www.atlassian.com/br/git/tutorials/what-is-git.
- https://git-scm.com/book/pt-br/v2/Come%C3%A7ando-Uma-Breve-Hist%C3%B3ria-do-Git
- HTML5. Devmedia, disponível em: [https://www.devmedia.com.br](https://www.devmedia.com.br/as-novidades-do-html5/23992). Acesso em: 28 de jan. de 2023.

# Como executar

Pré-requisitos: 
- Visual Studio Code
- GIT

```bash
# clonar repositório
git clone https://github.com/fbamuniz/class-04-jquery3.git

```

# Bibliografia das aulas

- DUCKETT, J. HTML e CSS: Projete e Construa Websites. Rio de Janeiro: Alta Books. 2016.
- MEYER, E. S. CSS – técnicas profissionais para um layout moderno. Porto Alegre: Bookman, 2011.


# Autor

Prof. Frederico Barbosa Muniz<br>
https://linktr.ee/fbamuniz
