---
title:  "GLFW: uma alternativa para o GLEW"
date:   2018-07-14 15:15:10 -0300
excerpt: GLFW é uma biblioteca de c++ para manipular entrada/saída.
categories: c++ c OpenGL
---

# Mas o que diabos é GLFW e GLEW?

Se você chegou aqui porque pegou o bonde já andando, recomendo ler o post sobre [OpenGL]({{ site.baseurl }}{% post_url 2018-07-14-introducao-ao-opengl %}). Mas se estiver com preguiça, trocando em miúdos é o seguinte: OpenGL é uma biblioteca para computação gráfica, mas ela não faz comunicação com os periféricos (monitor, input de teclado, etc), no workflow do OpenGL a biblioteca utilizada para gerenciar Input/Output é geralmente a GLEW do próprio Khronos Group, que desenvolve o OpenGL. Acontece que, diferente do OpenGL, o GLEW não é código aberto. Por isso estou escrevendo esse post para dar opções ao GLEW.

# Porque GLFW?

GLFW não é a única opção para quem é entusiasta do Open Source. Existe também uma versão Open Source do GLEW.

# Como usar

Documentação do [GLFW](http://www.glfw.org/docs/latest/quick.html#quick_steps)

{% highlight c++ %}
#include <GLFW/glfw3.h>

int main(int argc, char* argv[])
{

}

{% endhighlight %}

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
