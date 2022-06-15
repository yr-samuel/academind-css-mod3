### Propriedade Display

Por padrão os elementos HTML já vem com algum display definido, ou é __block__ ou __inline__, mas podemos alterar a propriedade display de qualquer elemento.

* Começando pelos elementos com display block, o seu comportamento é de sempre preencher o espaço total na horizontal do seu elemento pai, e sempre vai iniciar numa linha nova.

* Os elementos com display inline, o comportamento é de que sua largura sempre será relativa ao seu conteúdo, e sempre vai iniciar na mesma linha que outro elemento que tenha display inline.

  * Nos elementos inline até podemos definir um height, width, margin-top e margin-bottom, porém o elemento não sofrerá nenhuma dessa alterações.
  * Caso definamos algum padding-top ou bottom, esse espaçamento interno será inserido no elemento, mas não empurrará o conteudo que fica em volta, meio que ele ficará por cima dos outros conteúdos.
  * Somente quando o elemento ultrapassar os limites da largura do elemento pai que ele vai quebrar a linha e iniciar numa nova.
  * Não pode haver elementos com display block dentro de um elemento com display inline.

* É possível também definir a propriedade display com __inline-block__ que basicamente junta os comportamentos do __inline__ com o do __block__, com isso o elemento ainda continua sendo em linha, sua largura se mantém no tamanho do seu conteúdo, mas fica habilitado para modificarmos width, height, margin em sua totalidade e que realmente terá efeito real nesse elemento, o padding agora também empurrará os conteúdos que estão em volta.

* Quando definimos display __none__ para um elemento, ele é retirado da tela (vulgo fluxo dos elementos), porém não é removido do DOM.