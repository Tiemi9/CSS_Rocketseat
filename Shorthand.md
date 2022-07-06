# shorthand
- junção de propriedades
- resumido
- legível

'''CSS

{
    /*background properties*/

    background-color: #000;

    background-image: URL(image.bg.gif);

    backgroun-repeat: no-repeat;

    background-position: left top;}

    /*background shorthand*/

    background: #000 URL(image.bg.gif) no-repeat left top;





    /*font properties*/

    font-style: italic;

    font-weight: bold;

    font-side: 8em;

    line-height: 1.2;

    font-family: arial, sans-serif;

    /*font shorthand*/

    font: italic bold .8em/1.2 arial, sans-serif; (valores não especificados assume o padrão, ao alterar as propriedades o shothand não se altera e é o prevalecente)
}

# detalhes
- não considera prorpiedades anteriores
- valores não especificados assume o padrão
- geralmente a ordem não importa, porém se houverem muitos valores poderemos ter problemas.