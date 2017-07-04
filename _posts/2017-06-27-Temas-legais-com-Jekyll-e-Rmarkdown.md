---
layout: post
title:  Temas-legais-com-Jekyll-e-Rmarkdown
date: 2017-07-04 13:23:50
published: true
tags: [htmlwidgets, r]
---





O Jekyll possui um extenso sistema temático que permite alavancar diversos modelos e estilos disponibilizados e mantidos pela comunidade para personalizar a apresentação do seu site. 

Alguns desses temas podem ser encontrados nos sites:

* [http://jekyllthemes.org/](http://jekyllthemes.org/)
* [https://jekyllthemes.io/](https://jekyllthemes.io/)
* [https://github.com/jekyll/jekyll/wiki/Themes](https://github.com/jekyll/jekyll/wiki/Themes)
* [https://mademistakes.com/work/jekyll-themes/](https://mademistakes.com/work/jekyll-themes/)


O Jekyll possui um extenso sistema de temas que permite alavancar modelos e estilos. Os formulários organizam os layouts, includes e stylesheets de uma forma que podem ser substituídos pelo conteúdo desejado, para personalizar a apresentação do seu site. Nesse tutorial, começaremos com algumas dicas básicas, passando pelos temas, familiarizando-se com os diretórios/arquivos, e por fim mostraremos como alterar o tema de um site existente.

Antes de começarmos a modificar o site vamos conhecer a estrutura básica do site:

* **Layouts**
  + Refere-se a arquivos dentro do diretorio *_layouts*, estes definem a marcacao para o seu tema.
  
  
* **Includes**
  + Refere-se ao código dentro do diretório *_includes* que pode ser utilizado em vários layouts.
  
  
* **Sass**
  + Refere-se aos arquivos *.scss* no diretório *_sass* que define os estilos do tema.
  
  
* **Assets**
  + Refere-se a vários arquivos *assets* dentro do diretório. Contém o main.scss que importa arquivos *sass* dentro do diretório *_sass*. Iste *main.scss* é o processado na folha de estilo principal do tema *main.css* chamado *_layouts/default.html* via o *_includes/head.html*.
  
  + Este diretório pode incluir subdiretórios para gerenciar recursos de tipo similar, e será copiado como está, para o diretório de site que sofrerá a tranformação final.
  

Para alterar o tema do projeto, vamos utilizar o projeto do primeiro tutorial, [Jekyll Primeira Postagem](https://arthurlustosa.github.io/maisumsitesobre/). Após ter criado seu site utilizando o tutorial ele terá aseguinte aparência:

![Aparência Inicial](https://s11.postimg.org/cnc81725f/aparenciabase.png)

E terá a estrutura:


![Extrutura Inicial - retirada do tutorial: Jekyll Primeira Postagem](https://s7.postimg.org/kbg69glxn/estruturabase.png)

Os diretórios: *_includes*, *_layouts*, *_sass*, *assets* e o *css*, são os diretórios utilizados para definir o tema do seu site. Para modificar primeiro você deve fazer o download de um dos temas disponibilizados nos sites apresentados no início deste tutorial. Para este exemplo vamos utilizar o tema [jekyll-theme-libretto](http://jekyllthemes.org/themes/jekyll-theme-libretto/) disponibilizado no site [http://jekyllthemes.org/](http://jekyllthemes.org/).


![Tema Libretto](https://s9.postimg.org/e4dgu9oi7/libretto.png)

Após fazer o download de tema você deve seguir os seguintes passos:

* Extraia os arquivos dentro do .zip baixado. O tema libretto tem a seguinte estrutura:

![Estrutura Libretto](https://s24.postimg.org/luo0fbdbp/estruturalibretto.png)

* No diretório com os arquivos extraídos faça uma cópia dos diretórios *_includes*, *_layouts*, *_sass*, *assets* e *css*  que são disponibilizados;


* Acesse o diretório raiz do seu projeto (Primeiro Site) e cole/substitua os diretórios;


* Abra o seu projeto Rmarkdown + Jekyll e execute-o utilizando os comandos: *brocks::blog_gen()* e  *brocks::blog_serve()*. 


Ao executar o projeto se tudo ocorreu corretamente o site deverá ter o novo tema.

![Site com tema alterado](https://s12.postimg.org/hmzir4ikt/aparencianova.png)
