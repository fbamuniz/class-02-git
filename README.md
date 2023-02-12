# Git
![NPM](https://img.shields.io/npm/l/react)
# Introdução

Hoje o sistema de controle de versão mais usado e moderno do mundo é o Git. O Git é um projeto de código aberto, maduro e com manutenção ativa desenvolvido em 2005 por [Linus Torvalds](https://pt.wikipedia.org/wiki/Linus_Torvalds), o famoso criador do kernel do sistema operacional Linux. Um número impressionante de projetos de software depende do Git para controle de versão, incluindo projetos comerciais e de código-fonte aberto. Os desenvolvedores que trabalharam com o Git estão bem representados no pool de talentos de desenvolvimento de software disponíveis e funcionam bem em uma ampla variedade de sistemas operacionais e IDEs (Ambientes de Desenvolvimento Integrado).

Tendo uma arquitetura distribuída, o Git é um exemplo de [DVCS](https://en.wikipedia.org/wiki/Distributed_version_control) (Sistema de Controle de Versão Distribuído). Em vez de ter apenas um único local para o histórico completo da versão do software, como é comum em sistemas de controle de versão como o [CVS](https://pt.wikipedia.org/wiki/CVS) ou [SVN](https://pt.wikipedia.org/wiki/Subversion), no Git, a cópia de trabalho de todo desenvolvedor do código também é um repositório que pode conter o histórico completo de todas as alterações. Além de ser distribuído, o Git foi projetado com desempenho, segurança e flexibilidade em mente.

**Desempenho**

As características brutas de desempenho do Git são muito fortes quando comparadas a muitas alternativas. Fazer o commit de novas alterações, branches, mesclagem e comparação de versões anteriores – tudo é otimizado para desempenho. Os algoritmos implementados no Git aproveitam o conhecimento profundo sobre atributos comuns de árvores de arquivos de código-fonte reais, como costumam ser modificados ao longo do tempo e quais são os padrões de acesso. Diferente de alguns softwares de controle de versão, o Git não se deixa enganar pelos nomes dos arquivos ao determinar qual deve ser o armazenamento e o histórico de versões da árvore de arquivos. Em vez disso, o Git se concentra no conteúdo do arquivo. Afinal, os arquivos de código-fonte são renomeados, divididos e reorganizados com frequência. 

**Segurança** 

O Git foi projetado com a integridade do código-fonte gerenciado como uma prioridade. O conteúdo dos arquivos, bem como os verdadeiros relacionamentos entre arquivos e diretórios, versões, tags e commits, todos esses objetos no repositório do Git são protegidos com um algoritmo de [hash](https://pt.wikipedia.org/wiki/Fun%C3%A7%C3%A3o_hash) de criptografia seguro chamado [SHA1](https://pt.wikipedia.org/wiki/SHA-1). Isso protege o código e o histórico de alterações contra alterações acidentais e maliciosas e garante que o histórico tenha rastreabilidade total. Com o Git, você pode ter certeza de ter um histórico de conteúdo autêntico do código-fonte. Alguns outros sistemas de controle de versão não têm proteções contra alterações secretas posteriores. Isso pode ser uma vulnerabilidade séria de segurança das informações para qualquer empresa que depende do desenvolvimento de software.

**Flexibilidade**

Um dos principais objetivos de design do Git é a flexibilidade. O Git é flexível em vários aspectos: suporte a vários tipos de fluxos de trabalho de desenvolvimento não lineares, em eficiência em projetos pequenos e grandes e em compatibilidade com muitos sistemas e protocolos existentes. O Git foi projetado para tratar os branches e tags como cidadãos de primeira classe (ao contrário do SVN) e operações que afetam branches e tags (como mesclagem ou reversão) também são armazenadas como parte do histórico de alterações. Nem todos os sistemas de controle de versão apresentam esse nível de rastreamento.

## Por que usar o Git?

Atualmente o Git é a melhor escolha para a maioria das equipes de software. Embora cada equipe seja diferente e deva fazer a própria análise. O Git tem a funcionalidade, desempenho, segurança e flexibilidade que a maioria das equipes e desenvolvedores individuais precisam. Nas comparações lado a lado com a maioria das outras alternativas, muitas equipes acham que o Git é muito favorável.

Ele é atraente pelos seguintes motivos. Um grande número de desenvolvedores já tem experiência com o Git e uma proporção significativa de recém-formados pode ter experiência apenas com o Git. Embora algumas empresas precisem escalar a curva de aprendizado ao migrar para o Git de outro sistema de controle de versão, muitos desenvolvedores existentes e futuros não precisam ser treinados no Git.

Além dos benefícios de um grande conjunto de talentos, a predominância do Git também significa que muitas ferramentas e serviços de software de terceiros já estão integrados ao Git, incluindo IDEs e novas ferramentas de uso como o cliente de desktop DVCS Sourcetree, software de rastreamento de itens e projetos, Jira, e serviço de hospedagem de código, Bitbucket.

Se você é um desenvolvedor inexperiente que quer desenvolver habilidades valiosas em ferramentas de desenvolvimento de software, quando se trata de controle de versão, o Git deve ser um dos itens na lista. O Git é um projeto de código aberto muito bem suportado, com mais de uma década de administração sólida. Os mantenedores do projeto mostraram um equilibrado e uma abordagem madura para atender às necessidades de longo prazo dos usuários, com lançamentos regulares que melhoram a usabilidade e a funcionalidade. É fácil examinar a qualidade do software de código aberto e inúmeras empresas dependem muito dessa qualidade.

O Git tem excelente suporte da comunidade e uma vasta base de usuários. A documentação é excelente e abundante, incluindo livros, tutoriais e sites dedicados. Existem também podcasts e tutoriais em vídeo. O código aberto reduz o custo para desenvolvedores amadores, pois eles podem usar o Git sem pagar uma taxa. Para uso em projetos de código aberto, o Git é sem dúvida o sucessor das gerações anteriores de sistemas bem-sucedidos de controle de versão de código aberto, SVN e CVS.

Uma crítica comum ao Git é que pode ser difícil de aprender. Algumas das terminologias do Git vão ser novas para os iniciantes e, para usuários de outros sistemas, a terminologia do Git pode ser diferente, por exemplo, revert no Git tem um significado diferente do que no SVN ou CVS. No entanto, o Git é muito eficiente e disponibiliza muitos recursos aos usuários. Aprender a usar esses recursos pode levar algum tempo. No entanto, uma vez aprendidos, podem ser usados pela equipe para aumentar a velocidade de desenvolvimento.

Para as equipes que vêm de um VCS não distribuído, ter um repositório central pode parecer uma coisa boa que eles não querem perder. No entanto, embora o Git tenha sido projetado como um sistema de controle de versão distribuído (DVCS), com o Git, você ainda pode ter um repositório canônico oficial em que todas as alterações no software devem ser armazenadas. Com o Git, como o repositório de cada desenvolvedor está completo, o trabalho não precisa ser restringido pela disponibilidade e desempenho do servidor central. Durante interrupções ou quando offline, os desenvolvedores ainda podem consultar o histórico completo do projeto. Como o Git é flexível e está sendo distribuído, você pode trabalhar da maneira que está acostumado, mas obter os benefícios adicionais do Git, alguns dos quais você nem percebe que está perdendo.

### 1. Configurando seu computador local

Agora que você entendeu o que é o controle de versão, o que é o Git e por que as equipes de software deveriam optar por ele, vamos a prática! Considerando que você já [baixou o Git](https://git-scm.com/) e o Visual Studio Code, abra o prompt de comando (MS-DOS, Git ou no VSC) e execute os comandos abaixo: 

```bash
# Exibe a versão do Git que você instalou.
git version

# É preciso definir um user no Git.
git config --global user.name "Fred"

# Verifica o nome que você criou
git config user.name

# É preciso definir um e-mail no Git.
git config --global user.email "fred@fred.com"

# Verifica o e-mail que você criou
git config user.email
```

### 2. Baixando um repositório do Github no seu computador

Considerando que você já possui uma conta aqui no [Github](https://github.com), crie um projeto somente com os arquivos README e com uma licença MIT. Ao finalizar, você visualizará um botão chamado **Code**. Clique neste botão e copie a URL do diretório. Volte para o prompt do Git:

```bash
# Crie um diretório, baixe o projeto que você criou e abra no VSC
git clone https://github.com/user/project-name.git

```

### 3. Enviando um projeto local para o Github

Após ter criado e modificado os arquivos do seu projeto, agora você consegue envia-los para o diretório remoto do Github. Os comandos necessários para este procedimento são:

```bash
# Verifica quais itens sofreram modificações
git status

# Adiciona todas as alterações em um container local
git add .

# Faz o commit do container
git commit -m "Versão x.x"

# Envia as alterações para o Github
git push

```

### 4. Versionamento e Merge no mesmo computador

Uma das coisas mais legais do Github é criar versionamento e ramificações dos seus projetos . Abaixo, faremos um exemplo, considerando que duas pessoas (Ana e Julia) estão trabalhando em um mesmo projeto em um único computador. Baixe o plugin do VSC chamado Git Graph, isso facilitará a visualização das versões:

```bash
# Crie 3 versões, repetindo os passos do item 3. Em seguida, crie uma ramificação para Ana.
git checkout -b Ana

# Crie uma outra ramificação para Julia. Faça algumas alterações no projeto (item 3).
git checkout -b Julia

# Volte para a ramificação da Ana e faça algumas alterações.
git checkout Ana

# Você consegue verificar em qual ramificação está com o comando abaixo.
git branch

# Para realizar o merge é necessário voltar para a ramificação master. Faça também algumas alterações.
git checkout master

# Aglutine a ramificação master com Ana, resolva os conflitos no VSC e repita os passos do item 3.
git merge Ana

# Aglutine a ramificação master com Julia, resolva os conflitos no VSC e repita os passos do item 3.
git merge Julia

```

Observe no Git Graph que as versões da Ana e Julia, agora estão incorporadas na versão Master. 

### 4. Sincronizando dois ou mais projetos no Github

Outra coisa comum no Git são duas ou mais pessoas trabalhando no mesmo projeto remoto. Para o exemplo abaixo, imagine que Maria e Pedro baixaram o mesmo projeto do Github, fizeram alterações em seus computadores locais e agora desejam envia-los novamente para o repositório de origem. Para fazer esta simulação, usaremos um único computador, mas com dois diretórios distintos, um chamado Maria e outro Pedro. Precisaremos também de duas contas diferentes do Github, pois cada diretório será manipulado por um prompt diferente (ou você pode fazer com um amigo, por exemplo). Também vamos considerar que o projeto já está dentro de cada diretório, que você já fez algumas alterações e também já executou os passos do item 3 (com exceção do push) em cada cópia.

```bash
# Primeiramente, suba para o GitHub somente o projeto da Maria.
git push

# No diretório do Pedro, use o comando abaixo para baixar somente as alterações que Maria fez.
git fetch

# Verifique se você está no ramo origin (versão do Github).
git remote

# O comando abaixo baixará os novos arquivos da Maria, mas somente para análise.
git checkout origin

# Retorne ao ramo master
git checkout main

# Use o comando abaixo para resolver os conflitos. Na sequência, use os comandos do item 3.
git pull

# Para finalizar o sincronismo, abra a versão da Maria e use também o mesmo comando.
git pull

```

No exemplo acima, simulamos um projeto copiado por dois desenvolvedores, mas você pode trabalhar com "n" desenvolvedores no mesmo projeto, basta que todos sigam o mesmo procedimento listado acima.

## Considerações finais

O Github ainda possui alguns recursos que nos auxiliam no desenvolvimento de aplicações. Por exemplo, na opção **Settings > Pages** é possível hospedar gratuitamente uma página Web, desde que ela atenda aos requisitos da plataforma. Outro recurso interessante é o [Kanban](https://pt.wikipedia.org/wiki/Kanban) integrado ao repositório do projeto, que permite organizar melhor as tarefas e etapas a serem desenvolvidas. Há também a possibilidade de definir um tipo de liçensa especifica para cada projeto, por meio do arquivo License, além de customizar com o uso da linguagem [Markdown](https://docs.pipz.com/central-de-ajuda/learning-center/guia-basico-de-markdown#open) ou HTML o arquivo de descrição README.md.

No vídeo abaixo da Rafaella Ballerini, é apresentado um pequeno resumo do que é o Git e Github. 

[![Assista ao vídeo](https://img.youtube.com/vi/DqTITcMq68k/maxresdefault.jpg)](https://www.youtube.com/watch?v=DqTITcMq68k)

## Referências

- Git. Git-SCM, disponível em: [https://git-scm.com](https://git-scm.com/book/pt-br/v2/Come%C3%A7ando-Uma-Breve-Hist%C3%B3ria-do-Git). Acesso em: 11 de fev. de 2023.
- Git. Atlassian, disponível em: [https://www.atlassian.com](https://www.atlassian.com/br/git/tutorials/what-is-git). Acesso em: 11 de fev. de 2023.

## Como executar

Pré-requisitos: 
- Visual Studio Code
- GIT

```bash
# clonar repositório
git clone https://github.com/fbamuniz/class-07-git.git

```

## Bibliografia Básica 
- MEYER, E. S. CSS - técnicas profissionais para um layout moderno. Porto Alegre: Bookman, 2011.
- POWERS, S. Aprendendo JavaScript. São Paulo: Novatec, 2010.
- PETRUCELLI, E. E. HTML5, CSS e JavaScript. Brasília: NT Editora, 2019.
- DUCKETT, J. HTML e CSS: Projete e Construa Websites. Rio de Janeiro: Alta Books. 2016.
- SILVERMAN, R.E. Git: Guia prático. São Paulo: Novatec, 2019.
- GRINBERG, M. Desenvolvimento web com Flask: Desenvolvendo aplicações web com Python. São Paulo: Novatec, 2019.

## Bibliografia Complementar:
- GOMES, A. L. XHTML/CSS: criação de páginas web (Informática). São Paulo: Editora Senac, 2019.
- QUIERELLI, D. A. Criando sites com HTML-CSS-PHP: Construindo um projeto - Iniciante. Joinville: Clube dos Autores, 2012.
- TITTEL, E., NOBLE, J. HTML, XHTML e CSS Para Leigos. Rio de Janeiro: Alta Books, 2014

# Autor

Prof. Frederico Barbosa Muniz<br>
https://linktr.ee/fbamuniz