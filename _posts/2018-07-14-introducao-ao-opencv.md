---
layout: default
title:  "Introdução ao OpenCV"
author: Josivan Medeiros
date:   2018-07-14 15:15:10 -0300
excerpt: OpenCV é uma biblioteca escrita em C/C++ focada principalmente em Visão Computacional em tempo real. Ela é Multiplataforma e tem bindings para Java, Python e C++.
categories: processamento-de-imagem c++ Python Java
---

# O que é OpenCV

OpenCV é uma biblioteca escrita em C/C++ focada principalmente em Visão Computacional em tempo real. Ela é Multiplataforma e tem bindings para Java, Python e C++.

# Como instalar

A documentação do OpenCV recomenda que se utilize o cmake para a instalação. Se você não conhece o cmake e quer saber mais leia este [post](colocar aqui o post).
Você pode baixar o código fonte do OpenCV nesse link * insira aqui o link * para poder compilar e gerar o instalador.
Antes de executar o `cmake` é necessário instalar algumas bibliotecas que são dependencias para o OpenCV.
Uma das bibliotecas listada na documentação pode dar problema. Você precisará instalar uma versão anterior. Digite no terminal:

`echo "deb http://us.archive.ubuntu.com/ubuntu/ yakkety universe" | sudo tee -a /etc/apt/sources.list`

E então:

`sudo apt-get update`

`sudo apt-get install libjasper-dev`

Outra opção:

`sudo add-apt-repository "deb http://security.ubuntu.com/ubuntu xenial-security main"`

`sudo apt update`

`sudo apt install libjasper1 libjasper-dev`

Finalmente descompacte a pasta do opencv e dentro da pasta crie uma pasta `build`:

`mkdir build`

`cd build`

Dentro da pasta `build` digite o comando:

`cmake -D CMAKE_BUILD_TYPE=Release -D CMAKE_INSTALL_PREFIX=/usr/local ..`

Esse comando irá criar os arquivos necessários para a compilação. Ao terminar compile com:

`make -j7`

O parâmetro `-j7` significa que o processo irá utilizar 7 threads. Isso irá consumir bastante processamento do seu PC, mas a instalação será mais rápido. Se for executar outras tarefas enquanto instala (já que o processo é bem demorado) você pode diminuir o número de threds com `make -j5` ou `make -j4` por exemplo.
Finalmente, para instalar as bibliotecas digite:

`sudo make install`

# Como usar

Vamos ver um exemplo de um programa simples `DisplayImage.cpp` abaixo:

{% highlight c++ %}
#include <opencv2/opencv.hpp>

using namespace cv;

int main(int argc, char* argv[])
{

}

{% endhighlight %}

