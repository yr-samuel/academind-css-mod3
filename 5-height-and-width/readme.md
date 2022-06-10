### Width

* O comportamento padrão de elementos do tipo block é que a sua __largura__ preencha totalmente o espaço disponível do elemento pai, logo width desse tipo de elemento é sempre 100%.

* Não só de medidas relativas os elementos de bloco vivem, é totalmente possível usar medidas absolutas neles, como por exemplo: __200px__.

### Height

* Quando colocamos 100% de __altura__, percebemos que dependendo do caso não há nenhuma alteração no nosso elemento, pois esse elemento pega a referência da altura do seu elemento pai, e se esse elemento pai não tiver uma altura definida, nada acontecerá.

* Quando temos conteúdo dentro de um elemento, a sua altura é definida dinamicamente pela soma das alturas dos elementos filhos, mas quando tentamos setar uma altura em porcentagem para um elemento filho, nada acontece, pois como a altura do pai é calculada dinamicamente baseado na altura dos elementos filhos, isso entraria em um loop infinito.

* Se quisermos que nosso elemento tenha uma altura, ou passamos um valor que não seja referente a altura do elemento pai, ou setamos uma altura Absoluta para o elemento pai.