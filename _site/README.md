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

```

## Execução e exportação
Execute a página web gerada pelo jekyll com o seguinte comando
~~~shell
$
~~~