# JekyllDocs
Usando Jekyll para a geração de sites de documentação em linguagem de markdown. Abaixo está listado alguns passos para a instalação rápida do [Jekyll](https://jekyllrb.com/docs/):

## Instalação e configuração
Instalação e configuração e instalação do ambiente Ruby, mais informnações em [`Jekyll on Ubuntu`](https://jekyllrb.com/docs/installation/ubuntu/):
~~~shell
$ sudo apt-get install ruby-full build-essential zlib1g-dev
~~~
Configuração das variáveis de ambiente:

~~~shell
$ echo '# Install Ruby Gems to ~/gems' >> ~/.bashrc
$ echo 'export GEM_HOME="$HOME/gems"' >> ~/.bashrc
$ echo 'export PATH="$HOME/gems/bin:$PATH"' >> ~/.bashrc
$ source ~/.bashrc
~~~
Instalação do Jekyll:
~~~shell
$ gem install jekyll bundler
~~~

## Criação
Criação e configuração de uma nova página de documentação com Jekyll:
~~~shell
$ jekyll new docs
~~~
A estrura de pastas gerada pelo jekyll deve se parecer com:
```
_docs/
    _ _posts/
        |_2020-03-11-welcome-to-jekyll.markdown
    |_ _config.yml
    |_404.html
    |_about.markdown
    |_Gemfile
    |_index.markdown
```
Os arquivos em markdown podem ser tanto `.md` quanto `.rst` podendo configurar essas características no arquivo `_config.yml`, assim como o repositório do github a ser utilizado para edição e o estilo da página.
Os arquivos `.html` e `.css` podem ser customizados de acordo com a documentação do [Jekyll](https://jekyllrb.com/docs/).
As páginas em markdown devem possuir um cabeçalho para a configuração do comportamento da página, como se segue:
~~~yml
---
layout: page
title:  "Welcome to Jekyll!"
date:   2020-03-11 15:11:52 -0300
categories: jekyll update
---
~~~

## Execução e exportação
Execute a página web gerada pelo jekyll na pasta root do projeto `cd myblog` com o seguinte comando:
~~~shell
$ bundle exec jekyll serve
~~~
Digite no seu navegador o endereço [`localhost:4000`](http://localhost:4000/).