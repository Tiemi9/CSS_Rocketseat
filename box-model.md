# box model
-  fundamental para fazer layout para web
- maior facilidade para aplicar CSS

## o que é?
- uma caixa retangular
- essa caixa possiu propriedades de uma caixa 2D


'''CSS

- tamanho (largura x altura)        width/height

- contúdo                           content

- borda                             border

- preenchimento interno             padding

- espaços fora da caixa             margin

cada elemento na sua página, será considerado uma caixa

## box sizing
como será calculado o tamanho da caixa?
- content-box/border-box

'''css

div {
    box-sizing: border-box
    }
    
 ## 'diplay: block' vs 'display: inline'
 - como as caixas se comportam em relação a outras caixas
 - comportamento externo das caixas

 block:
 - ocupa toda a linha, colocando o próximo elemento abixo desse
 - width e height são respeitados
 - padding, margin, borde irão funcionar normalmente

 inline:
 - elemento ao lado
 - width e height não funcionam
 - somente valores horizontais de margin, paddin e border  

 ex.: 

 block '<p> <div> <section>', todos os headings '<h1> <h2>...'

 inline '<a> <strong> <span> <em>

 ## Margin
 Espaços entre elementos

 - margin-top  /  margin-right / margin-bottom / margin-left
 - values: '<length>' / '<percentagem>' / auto

 '''css

div {

    /*shorthand*/ (agrupamentos)
    margin: 12px 16px 10px 4px; (top, right, bottom, left)

    margin: 12px 16px 0; (top, sides, bottom)

    margin: 8px 16px; (top + bottom, sides)

    margin: 8xp; (todos iguais)

} 

CUIDADO COM MARGIN COLLAPSING (TOP SE JUNTO COM BOTTOM)

https://developer.mozila.org/en-us/doc/Web/CSS/margin

## Paddin
preenchimento interno da caixa

- padding-top / paddin-right / padding-bottom / padding-left
- values: '<lenght>' / '<percentagem>' / auto

'''css

div {
    
    /*shorthand*/ (agrupamentos)
    padding: 12px 16px 10px 4px; (top, right, bottom, left)

    padding: 12px 16px 0; (top, sides, bottom)

    padding: 8px 16px; (top + bottom, sides)

    padding: 8xp; (todos iguais)
    
}

PADDING PODERÁ CAUSAR DIFERENÇA NA LARGURA DE UM ELEMENTO

https://developer.mozila.org/en-us/doc/Web/CSS/PADDIN

## border e outline
as bordas da caixa

- value: '<border-style>' / '<border-width>' / '<border-color>'
        - Style: solid, dotted, dashed, double, groove, ridge, inset, outset
        - width: '<lenght>'
        - color: '<color>'

'''css

div {
    border-top-width: 2xp

    - /*shothand pois poderia ser escrito:
    border-top-width: 2px*/
    border-top: solid 2 px; /* top, right, bottom, left*/

    - /*style*/
    border: solid

    - /*width '<length>' / style*/
    border: 2ps dottted;

    - /*style/color*/
    border: outset #f33;

    - /*width/style/color*/
    border: medium dashed green;
}

### Outline
O outline é muito semelhante ao border, mas difere em 4 sentidos:
- Não modifica o tamanho da caixa, pois não é parte do Box Model
- Poderá ser diferente de retangular
- Não permite ajuste individuais
- Mais usado pelo user agent para acessibilidade

https://developer.mozilla.org/en-US/docs/Web/CSS/border                                