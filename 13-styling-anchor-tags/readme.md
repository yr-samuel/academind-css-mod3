### Styling Anchor Tags

* Aqui foi estilizado as tags \<a>, colocando a cor <span style="color: #0e4f1f;">verde</span> para a letra, e foi removido o text-decoration passando __none__.

* Também queriamos espaçar cada item da lista, na aula é colocado __margin: 0 16px;__ porém dessa forma ficará um espaço gigantesco entre os elementos que estão entre outros elementos, e para resolver isso, usei a técnica de combinação de seletores que só aplica o estilo caso aquele seletor seja precedido do outro seletor especificado, no caso coloquei caso o item da lista fosse precedido de outro item da lista colocava um __margin-left: 16px;__
  
  > .main-nav__item + .main-nav__item { margin-left: 16px }