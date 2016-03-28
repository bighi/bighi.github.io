---
layout: post
title: Como Eu Organizo Minha Vida Em TXT
tags: [plaintext, markdown]
excerpt: Onde eu explico como organizo minhas anotações, tarefas e documentos usando apenas arquivos simples em diretórios.
image:
  feature:
date: 2015-12-12T08:28:47-02:00
---

Ontem eu falei sobre meu problemas com formatos proprietários para anotar
informação.  Agora é hora de explicar como eu organizo minhas notas, arquivos,
documentos, tarefas, etc.

Lembrando que uso apenas arquivos simples (txt para anotações) em diretórios
sincronizados com Dropbox.

Nesse sistema eu guardo as seguintes informações:

- Notas de acesso frequente
- Referências que posso precisar algum dia
- Notas de projetos passados em que não trabalho mais
- Minhas tarefas que preciso fazer
- As tarefas que fiz
- Meu diário
- Documentos diversos

## Como eu organizo as notas ##

Eu tenho várias notas. Eu anoto qualquer informação que eu precise lembrar, ou
que possa ser útil no futuro. Placa do meu carro, IMEI do meu telefone, ideias
que eu tive pra um livro, uma série que um amigo sugeriu, comandos de terminal
que eu sempre esqueço, etc.

Primeiro de tudo, todas as minhas anotações ficam dentro do diretório
~/Dropbox/Notes.

### Tipos de notas ###

Eu classifico minhas anotações em dois tipos: notas e referências.

Referências são informações que estão lá caso eu precise algum dia, mas eu
raramente acesso.  Exemplos: placa do meu carro, IP dos dispositivos da minha
casa, dados dos celulares, números de documentos.

Notas são anotações gerais que não estão lá apenas para referência. São coisas
que eu vou acessar (e editar) com maior frequência.  Exemplos: listas de ideias,
coisas que me recomendaram, itens que preciso comprar no mercado, coisas que
emprestei pra alguém.

### Projetos ###

Além disso, as anotações podem se referir a um projeto específico ou não.

Quando eu estou anotando informações que só dizem respeito a um projeto, não faz
sentido deixar isso junto do resto. Eu crio um diretório com o nome do projeto,
dentro do diretório Notes, e guardo os arquivos dele lá dentro.

Faço isso com projetos do trabalho, ou um projeto pessoal meu que eu acho que
vai dar dinheiro. Não faz sentido para projetos curtos que não vão ter vários
arquivos.

Quando o projeto está terminado e não preciso mais das notas, eu movo o
diretório inteiro para dentro de um outro diretório chamado Arquivados.
Provavelmente eu nunca mais vou ler novamente aquelas notas, mas pelo menos
tenho a informação guardada caso eu precise.

Apesar dessa organização, é importante deixar claro que **a grande maioria das
minhas anotações fica apenas no diretório Notes, sem estar dentro de nenhum
diretório de projeto.**

### Markdown ###

Independente de ser uma Nota ou Referência, de assunto geral ou projeto, todas
elas são formatadas num estilo chamado Markdown.

Markdown é uma forma de escrever textos puros que permite que o texto seja
transformado em HTML quando você quiser vê-lo de uma forma mais bonitinha.

Ele faz isso sem deixar o texto ilegível e cheio de código, e de uma forma que
seja fácil de ler mesmo olhando para o texto puro.

O Markdown usa algumas marcações no texto, como \*\*negrito\*\*, ou \_itálico\_.
Ou outras marcações para links, cabeçalhos, tabelas, etc.

Essa é a melhor forma de ter texto puro, mas ainda com um potencial de ser um
texto rico que fica bonito quando você precisa.

## Como eu organizo as tarefas ##

Todas as minhas tarefas também ficam em um arquivo de texto. Eu tenho um arquivo
chamado todo.txt que segue uma sintaxe que também se chama
[**Todo.txt**][todotxt]. Você pode ler mais sobre essa sintaxe [aqui][todotxt].

A ideia é simples: cada linha no arquivo de texto é uma tarefa. As tarefas podem
receber um @contexto marcado com arroba, e fazer parte de +projetos marcados com
um sinal de + antes do nome.

Além disso, podem ter a prioridade no começo da linha entre parênteses. A
prioridade começa em A, depois B, depois C, e por aí vai.

Exemplo:

```
(A) Limpar as manchas de sangue @casa +cadáver
(B) Esconder o corpo @casa +cadáver
(C) Anunciar minha motosserra no Mercado Livre @computador +cadáver
Procurar nova pessoa pra dividir o apartamento comigo +apartamento
Comprar novo abajur @mercado
```

Anotando dessa forma, eu posso ver e editar minhas tarefas em qualquer editor de
texto. Mas também posso usar os aplicativos específicos para Todo.txt, quando eu
quiser ver minhas tarefas numa interface própria pra isso.

Esse é mais um grande exemplo de como eu posso usar um aplicativo próprio para
fazer alguma coisa, mas ainda tenho o arquivo num formato livre e sem ficar
preso no servidor de alguma empresa.

Existem aplicativos de Todo.txt para [iOS][todo-ios] e [Android][todo-android],
assim como Windows, Mac e Linux.

### As tarefas concluídas ###

Existe mais uma coisa que o Todo.txt faz. Ele move as tarefas concluídas para um
diretório chamado done.txt, colocando no começo da linha a data em que a tarefa
foi concluída. Assim ele não polui a lista de tarefas principal, mas mantém um
histórico de tarefas concluídas caso você precise consultar.

Se você quiser fazer reviews semanais ou mensais, pode fazer um script que
vasculha o done.txt procurando pelas tarefas com data da última semana ou mês.

## Como organizo meu diário ##

Isso não vai ser nenhuma surpresa, mas meu diário também fica salvo num arquivo
de texto simples. Desta vez, ele é gerenciado por outro programa, um aplicativo
de terminal chamado [**jrnl**][jrnl].

O jrnl oferece vários comandos que tornam muito prático fazer anotações no
diário e rever as entradas com filtros de data.

E no fim das contas é apenas um arquivo journal.txt com datas e texto.

## Documentos diversos ##

Por último, eu gosto de ter cópias de todos os meus documentos de uma forma
fácil de acessar. Tanto documentos pessoais (RG, CPF, título de eleitor, etc)
quanto extratos mensais do banco, contracheques e notas fiscais de produtos.

Esse tipo de arquivo não tem jeito, eu preciso de um formato visual.

O mais próximo de um formato aberto que vai durar por muito tempo é o PDF. Ele
permite imagens e texto, incluindo a possibilidade ter o texto escaneado da
imagem e incluído no arquivo pra que fique uma imagem com texto selecionável.

Então todos os meus documentos em papel são escaneados, tem os caracteres
reconhecidos por algum aplicativo de OCR, e são salvos num diretório chamado
"Arquivo Digital".

## Aplicativos que eu uso ##

No Android, eu uso [**Neutrinote**][neutrinote] para editar as notas, e o
[**Todo.txt**][todo-android] para gerenciar as tarefas.

No Linux, eu uso o [**Vim**][vim] para editar notas, e o
[**QTodoTxt**][qtodotxt] para gerenciar as tarefas.

No Mac, eu uso [**Notational Velocity**][nvalt] para minhas anotações gerais,
[**Marked**][marked] para ler arquivos de texto em Markdown, e a versão de
console do Todo.txt para gerenciar as tarefas.

## Tudo está a poucos clique de distância ##

Existe algo em comum entre todos esses tipo de documentos que guardo:

1) Todos estão sempre disponíveis pra mim, seja em casa, no trabalho ou na rua.

2) Eu posso acessar de qualquer dispositivo. Seja um computador, celular, ou até
mesmo no meu smartwatch. 

3) Vão continuar acessíveis por anos, não importa
quais empresas fechem ou que servidores explodam.

Se a característica mais importante de um sistema de notas é estar disponível
quando eu preciso, eu posso dizer que meu sistema é um sucesso.

## Mantendo um histórico por muitos anos ##

Eu só estou fazendo todo este esforço porque quero passar a manter um histórico
da minha vida por muitos e muitos anos. Eu gostaria muito de ter feito isso
desde novo, mas agora é tarde para pensar nisso.

Mas eu quero poder olhar daqui a 5 anos e ver que tarefas eu estava fazendo
hoje, ou ler o diário e ver quais eram meus objetivos, sonhos e problemas.

O que quer que eu queira fazer, eu sei que os arquivos estarão lá esperando por
mim.

[todotxt]:http://todotxt.com
[todo-ios]:http://itunes.apple.com/br/app/todo.txt-touch/id491342186?ls=1&mt=8
[todo-android]:http://play.google.com/store/apps/details?id=com.todotxt.todotxttouch
[jrnl]:https://github.com/maebert/jrnl
[neutrinote]:https://play.google.com/store/apps/details?id=com.appmindlab.nano&hl=pt_BR
[vim]:http://www.vim.org
[qtodotxt]:https://github.com/QTodoTxt/QTodoTxt
[nvalt]:http://brettterpstra.com/projects/nvalt/
[marked]:http://marked2app.com/
