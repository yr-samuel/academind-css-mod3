### Box Sizing

* Por padrão, o box-sizing de qualquer elemento é o __content-box__, então acontece que quando definimos um width e/ou height, ele será aplicado ao conteúdo do elemento, e não a caixa (box) toda. E então, quando colocamos border e padding, o tamanho do elemento não fica como esperado, pois o seu tamanho é calculado somando width e height + border + padding.
    > Então, caso tivessemos um height e width de 200px, border 1px e padding de 10px, o nosso elemento acabaria com um height e width de 222px.

* Para resolver esse problema, podemos passar para a propriedade __box-sizing__ o valor *border-box*, que então fará o cálculo do tamanho do nosso elemento incluindo o padding e o border que aplicamos. 
    > Então, caso coloquemos height e width de 200px, border 1px e padding de 10px, o nosso elemento vai acabar com o tamanho esperado de 200px tanto de height quanto width.
    
    > Isso acontece, pois o box-border, vai fazer um cálculo tanto do width e do height subtraindo o valor de border e padding, e depois para dar o tamanho do elemento ele somará o border + padding, ficando com o tamanho que voce especificou no height e/ou width.

        > elementHeight = (height - padding - border) + padding + border
        > elementWidth = (width - padding - border) + padding + border

* Por convenção e menos dor de cabeça, a comunidade ja adota a ideia de colocar no CSS reset, colocar o box-sizing como border-box;

    
