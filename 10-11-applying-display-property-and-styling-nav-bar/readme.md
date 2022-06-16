### Aplicação da propriedade display e estilização da barra de navegação

* O objetivo era criar uma barra de navegação na horizontal, então primeiramente, deixamos alguns elementos de dentro da __.main-header__ como **inline-block**.

* Em seguida queriamos deixar o conteúdo da __.main-nav__ no canto direito da __.main-header__, e para isso foi necessário colocar o __width__ do nav como 100%, pois como ele é inline a largura é referente ao espaço que seu conteúdo ocupa, após definirmos 100% de width, vimos que houve uma quebra de linha, pois como ele ta 100% e já tem o elemento do nome do site, ultrapassou o espaço limite daquela linha, e para deixarmos tudo numa mesma linha foi feito um calc no elemento nav, 100% - a largura do elemento do nome da empresa.

* Porém aqui, acontece uma coisa engraçada, mesmo fazendo esse cálculo, as coisas não ficaram na mesma linha, e isso acontece pois quando os elementos são __inline__ ou __inline-block__ qualquer espaço que tenha entre esse elemento e outro no código, conta como espaço na tela, então para resolver isso por hora, foi removido as quebras de linha ou espaços no código HTML.

* Após isso, posicionamos o conteúdo da nav para a direita, e aqui está um aprendizado, quando os elementos são inline ou inline-block, podem também ser alinhados com a propriedade text-align __(__ aqui usamos text-align: right; __)__, só fica um aviso, o mesmo efeito pode acontecer com elementos de bloco, mas na verdade é que os elementos de bloco herdam essa propriedade um do outro até chegar no conteúdo, então acaba por ter o mesmo efeito.

* Outro aprendizado é que, dentro de uma lista (ul) tem os list items (li), como normalmente, porém dentro de uma lista, se quiser podemos colocar qualquer elemento, e para que esse elemento tenha o ::marker (pontinho) também, é necessário que o display dele seja list-item.