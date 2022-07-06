# distância absoluta <length>

são fixas e não alteram o valor
{
unidades    nome                equivalência

cm          Centímetros         1cm = 96px/2.54

in          inches (polegadas)  1in = 2.54cm = 96px

px          pixels              1px = 1/96th of 1in

}

- o mais comum é px
- não recomendado usar cm

# distância relativa
Relativas a outro valor, como elemento ppai, root ou tamanho da tela.
- maior adaptação a diferentes tipos de tela

unidade     relativo à
em          tamanho da fonte pai
rem         tamanho da fonte do elemento raiz (root/html)
vw          1% da viewport ("tela") width (largura)
vh          1% da viweport height (altura)
