# Git
![NPM](https://img.shields.io/npm/l/react)
# Introdução

O sistema de controle de versão moderno mais usado no mundo hoje é o Git. O Git é um projeto de código aberto maduro e com manutenção ativa desenvolvido em 2005 por [Linus Torvalds](#), o famoso criador do kernel do sistema operacional Linux. Um número impressionante de projetos de software depende do Git para controle de versão, incluindo projetos comerciais e de código-fonte aberto. Os desenvolvedores que trabalharam com o Git estão bem representados no pool de talentos de desenvolvimento de software disponíveis e funcionam bem em uma ampla variedade de sistemas operacionais e IDEs (Ambientes de Desenvolvimento Integrado).

Tendo uma arquitetura distribuída, o Git é um exemplo de [DVCS](#) (Sistema de Controle de Versão Distribuído). Em vez de ter apenas um único local para o histórico completo da versão do software, como é comum em sistemas de controle de versão como o [CVS](#) ou [SVN](#), no Git, a cópia de trabalho de todo desenvolvedor do código também é um repositório que pode conter o histórico completo de todas as alterações. Além de ser distribuído, o Git foi projetado com desempenho, segurança e flexibilidade em mente.

**Desempenho**

As características brutas de desempenho do Git são muito fortes quando comparadas a muitas alternativas. Fazer o commit de novas alterações, branches, mesclagem e comparação de versões anteriores – tudo é otimizado para desempenho. Os algoritmos implementados no Git aproveitam o conhecimento profundo sobre atributos comuns de árvores de arquivos de código-fonte reais, como costumam ser modificados ao longo do tempo e quais são os padrões de acesso. Diferente de alguns softwares de controle de versão, o Git não se deixa enganar pelos nomes dos arquivos ao determinar qual deve ser o armazenamento e o histórico de versões da árvore de arquivos. Em vez disso, o Git se concentra no conteúdo do arquivo. Afinal, os arquivos de código-fonte são renomeados, divididos e reorganizados com frequência. O formato do objeto dos arquivos de repositório do Git usa uma combinação de codificação delta (armazenamento de diferenças de conteúdo) e compactação e armazena com clareza o conteúdo do diretório e os objetos de metadados da versão.

**Segurança** 

O Git foi projetado com a integridade do código-fonte gerenciado como uma prioridade. O conteúdo dos arquivos, bem como os verdadeiros relacionamentos entre arquivos e diretórios, versões, tags e commits, todos esses objetos no repositório do Git são protegidos com um algoritmo de [hash](#) de criptografia seguro chamado [SHA1](#). Isso protege o código e o histórico de alterações contra alterações acidentais e maliciosas e garante que o histórico tenha rastreabilidade total. Com o Git, você pode ter certeza de ter um histórico de conteúdo autêntico do código-fonte. Alguns outros sistemas de controle de versão não têm proteções contra alterações secretas posteriores. Isso pode ser uma vulnerabilidade séria de segurança das informações para qualquer empresa que depende do desenvolvimento de software.

**Flexibilidade**

Um dos principais objetivos de design do Git é a flexibilidade. O Git é flexível em vários aspectos: suporte a vários tipos de fluxos de trabalho de desenvolvimento não lineares, em eficiência em projetos pequenos e grandes e em compatibilidade com muitos sistemas e protocolos existentes. O Git foi projetado para tratar os branches e tags como cidadãos de primeira classe (ao contrário do SVN) e operações que afetam branches e tags (como mesclagem ou reversão) também são armazenadas como parte do histórico de alterações. Nem todos os sistemas de controle de versão apresentam esse nível de rastreamento.

## Por que usar o Git?

Hoje, o Git é a melhor escolha para a maioria das equipes de software. Embora cada equipe seja diferente e deva fazer a própria análise. O Git tem a funcionalidade, desempenho, segurança e flexibilidade que a maioria das equipes e desenvolvedores individuais precisa. Esses atributos do Git são explicados acima. Nas comparações lado a lado com a maioria das outras alternativas, muitas equipes acham que o Git é muito favorável.

O Git é a ferramenta mais adotada da categoria. Ele é atraente pelos seguintes motivos. Um grande número de desenvolvedores já tem experiência com o Git e uma proporção significativa de recém-formados pode ter experiência apenas com o Git. Embora algumas empresas precisem escalar a curva de aprendizado ao migrar para o Git de outro sistema de controle de versão, muitos desenvolvedores existentes e futuros não precisam ser treinados no Git.

Além dos benefícios de um grande conjunto de talentos, a predominância do Git também significa que muitas ferramentas e serviços de software de terceiros já estão integrados ao Git, incluindo IDEs e novas ferramentas de uso como o cliente de desktop DVCS Sourcetree, software de rastreamento de itens e projetos, Jira, e serviço de hospedagem de código, Bitbucket.

Se você é um desenvolvedor inexperiente que quer desenvolver habilidades valiosas em ferramentas de desenvolvimento de software, quando se trata de controle de versão, o Git deve ser um dos itens na lista. O Git é um projeto de código aberto muito bem suportado, com mais de uma década de administração sólida. Os mantenedores do projeto mostraram um julgamento equilibrado e uma abordagem madura para atender às necessidades de longo prazo dos usuários, com lançamentos regulares que melhoram a usabilidade e a funcionalidade. É fácil examinar a qualidade do software de código aberto, e inúmeras empresas dependem muito dessa qualidade.

O Git tem excelente suporte da comunidade e uma vasta base de usuários. A documentação é excelente e abundante, incluindo livros, tutoriais e sites dedicados. Existem também podcasts e tutoriais em vídeo. O código aberto reduz o custo para desenvolvedores amadores, pois eles podem usar o Git sem pagar uma taxa. Para uso em projetos de código aberto, o Git é sem dúvida o sucessor das gerações anteriores de sistemas bem-sucedidos de controle de versão de código aberto, SVN e CVS.

Uma crítica comum ao Git é que pode ser difícil de aprender. Algumas das terminologias do Git vão ser novas para os iniciantes e, para usuários de outros sistemas, a terminologia do Git pode ser diferente, por exemplo, revert no Git tem um significado diferente do que no SVN ou CVS. No entanto, o Git é muito capaz e disponibiliza muitos recursos aos usuários. Aprender a usar esses recursos pode levar algum tempo. No entanto, uma vez aprendidos, podem ser usados pela equipe para aumentar a velocidade de desenvolvimento.

Para as equipes que vêm de um VCS não distribuído, ter um repositório central pode parecer uma coisa boa que eles não querem perder. No entanto, embora o Git tenha sido projetado como um sistema de controle de versão distribuído (DVCS), com o Git, você ainda pode ter um repositório canônico oficial em que todas as alterações no software devem ser armazenadas. Com o Git, como o repositório de cada desenvolvedor está completo, o trabalho não precisa ser restringido pela disponibilidade e desempenho do servidor "central". Durante interrupções ou quando offline, os desenvolvedores ainda podem consultar o histórico completo do projeto. Como o Git é flexível e está sendo distribuído, você pode trabalhar da maneira que está acostumado, mas obter os benefícios adicionais do Git, alguns dos quais você nem percebe que está perdendo.

### 1. Configurando seu computador local

Agora que você entendeu o que é o controle de versão, o que é o Git e por que as equipes de software deveriam optar por ele, vamos a prática! Considerando que você já [baixou o Git](#) e o [Visual Studio Code](), abra o prompt de comando (MS-DOS, Git ou no VSC) e execute os comandos abaixo: 

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

Considerando que você já possui uma conta aqui no [Github](#), crie um projeto somente com os arquivos README e com uma [licença MIT](#). Ao finalizar, você visualizará um botão chamado **Code**. Clique neste botão e copie a [URL](#) do diretório. Volte para o prompt do Git:

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

Retornando ao Github, você verá que as alterações locais foram enviadas para o seu repositório remoto.


No vídeo abaixo da Rafaella Ballerini, é apresentado um pequeno resumo do que é o Git e Github. 

[![Assista ao vídeo](https://img.youtube.com/vi/DqTITcMq68k/maxresdefault.jpg)](https://www.youtube.com/watch?v=DqTITcMq68k)

## Referências

- Git. Git-SCM, disponível em: https://git-scm.com/book/pt-br/v2/Come%C3%A7ando-Uma-Breve-Hist%C3%B3ria-do-Git. Acesso em: 11 de fev. de 2023.
- Git. Atlassian, disponível em: https://www.atlassian.com/br/git/tutorials/what-is-git. Acesso em: 11 de fev. de 2023.

# Como executar

Pré-requisitos: 
- Visual Studio Code
- GIT


# Bibliografia das aulas

- DUCKETT, J. HTML e CSS: Projete e Construa Websites. Rio de Janeiro: Alta Books. 2016.
- MEYER, E. S. CSS – técnicas profissionais para um layout moderno. Porto Alegre: Bookman, 2011.


# Autor

Prof. Frederico Barbosa Muniz<br>
https://linktr.ee/fbamuniz
