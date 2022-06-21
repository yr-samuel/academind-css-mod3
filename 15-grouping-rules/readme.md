### Agrupando regras CSS

* Quando mais de uma regra CSS tem os mesmos estilos CSS, faz sentido agrupá-las juntando os seletores, separado-os por vírgula e recebendo o estilo que é igual pra todos.

        .main-nav__item > a:hover {
            color: #fff;
        }

        .main-nav__item > a:active {
            color: #fff;
        }

    Isso pode vir a se tornar o seguinte grupo:

        .main-nav__item > a:hover,
        .main-nav__item > a:active {    
            color: #fff;  
        }