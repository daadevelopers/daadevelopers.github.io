---
title: Criando um Blog com o HEXO
date: 2017-08-24 21:24:05
tags: hexo
---

![logo-hexo](https://hexo.io/icon/apple-touch-icon-114x114.png "Logo Hexo")
O hexo é um novo framework para criação de blogs estaticos, de simples manutenção e super rapido, assim como a descrição do proprio [Site Oficial](https://hexo.io/ "Hexo: Rápido, simples e poderoso") diz: `A fast, simple & powerful blog framework`
<!--more-->
Para usar é necessario ter o nodejs instalado, depois é so baixar o hexo e começar a usar
```
npm install hexo-cli -g
hexo init blog
cd blog
npm install
hexo server
```
Com isso o hexo ja irá iniciar um servidor na porta 4000 e é so acessar no navegador o link `http://localhost:4000/`

para criar posts, você so tem que digitar
```
hexo new "Titulo do post ou o nome que quiser"
```
Você vai perceber que criou um novo arquivo com o nome que você colocou dentro da pasta `source/_posts/`

Para gerar os arquivos estáticos, você so deve rodar o comando
```
hexo generate
```
## Deploy
Agora vem uma das partes mais legais do hexo, com ele você pode exporta diretamente para o github pages(e outros lugares também), primeiro instale a dependencia
```
npm install hexo-deployer-git --save
```
agora so tem que configura o arquivo `_config.yml` assim:
```
deploy:
  type: git
  repository: git@github.com:daadevelopers/daadevelopers.github.io.git
```
Troque para o seu repositorio ;)

## Domínio Proprio
E para finalizar, se você ja tiver um dominio registrado ou querer usar um, basta criar um arquivo `CNAME` no diretorio `source` e dentro do arquivo coloque a url do seu dominio, exemplo:
```
echo "daadevelopers.com.br" > CNAME
```
Agora no site do registro br vc vai em editar zona e depois adicione o tipo `A` e o endereço `192.30.252.153`, depois repita o processo e adicione o endereço, `192.30.252.154` e por ultimo mode o tipo para `CNAME` e coloque a url do seu repositorio do git pages `daadevelopers.github.io`, pronto tudo em perfeito estado.

Para melhores referencias acessem o [site oficial do hexo](https://hexo.io/ "Hexo: Rápido, simples e poderoso").
