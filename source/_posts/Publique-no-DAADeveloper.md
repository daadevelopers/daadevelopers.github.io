---
title: Publique no DAADeveloper
date: 2017-08-29 21:57:15
categories: 
- github
tags: 
- github
author: Walter Nascimento Barroso
---
O DAADeveloper, é um grupo do qual programadores, espalhados por todos os lugares, usam para divulgar seus conhecimentos, se você deseja contribuir tambem, bastar segui as dicas...
<!--more-->
## Ambiente
Antes de tudo é necessario que você tenha o ambiente funcionando para isso aprenda pelo menos o basico sobre o [Hexo](https://hexo.io/ "Hexo: Rápido, simples e poderoso")
Depois é necessario que tenha uma conta no [GitHub](https://github.com/)
## Contribuindo
Agora com o ambiente funcionando, e conta no github, faça um fork do projeto, e baixe em sua maquina, após confirmar que esta tudo funcionando faça referencia ao projeto original
```
git remote add upstream git@github.com:daadevelopers/daadevelopers.github.io.git
```
Agora crie seu post, ou faça sua correção, comite e envie, perceba que por padrão utilizamos o branch development para o codigo fonte e o master para o deploy.
## Enviando
Após todo o processo e comite feito, atualize seu repositorio
```
git fetch upstream
git rebase upstream/development
git push -f origin development
```
## Solicite um "PULL REQUEST"
Com as alterações já foram enviadas para o seu repositório no GitHub, envie um "pull request" ao mantenedor.
Para isso vá a sua página no GitHub e clique em "Pull Request", será aberta uma página para que você descreva algum comentário para o mantenedor, preencha os campos e clique em "send Pull Request".
Pronto, agora é so esperar ser aceito.
