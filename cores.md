# cores
Usamos CSS p/ alterar cores em nosso documento

## tipos:
- background-color (p/ caixas)
- color (p/ textos)
border-color (p/ caixas)
- outros...

## valores
podemos definir s valores por:
- palavra-chave (blue. transparent)
- hexadecimal (#990011)
- funções: rgb, hsl, hsla

'''css

element

### /*keybord value*/

color: currentcolor;

### /*<named-color> values*/

color: red

color: orange

color: tan;

color: rebeccapurple

### /*<hex-color> values 0-F*/

color: #090; /*red green blue*/

color: #009900;

color: #090a;

color: #009900aa;

- variação de 0 à F
- se houver quarto bloco (alfa) indicara a transparência
- sempre uusar #no inicio

### /*<rgb()> values*/

color: rgb(34, 12, 64, 0.6);

color: rgba(34, 12, 64, 0.6);

color: rgb(34 12 64 / 0.6);

color: rgba(34 12 64 / 0,3);

color: rgb(34.0 12 64 / 60%);

color: rgba(34,6 12 64 / 30%);

- variação de 0 a 255
- 0 super preto e 255 maior incidencia da cor do momento
- se houver quarto bloco (alfa) indicara a transparência
- poderá ser representado de qualquer uma das formas acima.

### /*<hsl()> values

color: hsl(30, 100%, 50%, 0.6); /*hue - saturation - luminance*/

color: hsla(30, 100%, 50%, 0.6);

color: hsl(30 100%, 50%, 0.6);

color: hsla(30 100% 50% / 0.6);

color: hsl(30.0 100% 50% / 60%);

color: hsla(30,2 100% 50% / 60%);

- como coordenadas da paleta de cores, é determinado pela posição rgb em angulos de 0° à 360°, sendo 0° red, 120° green e 240° verde.
- a posição da cor na paleta é presentada no primeiro campo
- segundo campo indica porcentagem de saturação, onde 0 é branco
- terceiro campo indica luz, onde 0 sem luz e 100 superbranco
- quarto campo indica tranparência

### /* global values*/

color: inherit; (cor de herança, herda cor do elemento anterior)

color: initial; (cor inicial, volta cor inicial)

color: current-color; (pega cor do contexto, mesma coisa que não colocar)

color: unset; (não estou definindo cor)


https://developer.mozilla.org/en-US/docs/Web/CSS/color_value

convert a color (site)