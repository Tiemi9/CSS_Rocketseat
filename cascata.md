# A cascata (cascading)
- A escolha do browser de qual regra aplicar, caso haja muitas regras para o mesmo elemento.
    - seu estilo é lido de cima para baixo

Consideramos 3 fatores:

- Origem do estilo
- Especificidade
- Importância

### Origem do estilo (ordem de força)
inline > tag style > tag link
- elemento style dentro da tag '<x style="">
- tag style '<style></style>'
- link do CSS  '<link rel="stylesheet" href="style.css">'

### Especificidade
É um cáuculo matemático, onde, cada tipo de seletor e origem do estilo, possuem valores a serem considerados.
0. Universal selector (*), combinators, e negation pseudo-class (:not))
1. Element type selector e pseudo-elements (:: before, ::after)
10. Classes e atribute selectors ((type="radio"))
100. ID selector
1000. inline


### A Regra IMPORTANT 
'x{ color: y, !impotant;' 

Sobressai a todas as ordens descritas acima
- cuidado evite o uso
- não é considerado uma boa prática
- quebra o fluxo natural da cascata

