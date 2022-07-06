# introdução

## O que significa CSS
 - Cascading Style Sheet
 - Código para criar estilos no HTML
 - Dá beleza
 - Não é linguagem de programação e sim de Style Sheet.

 # Comentários
- Não afeta o cód
- ajuda a lembrar blocos de código
- deixa dicas para leitura
- ajuda outros a entenderem
- Não esquecer de fechar o comentário
Comentarios começam com '/*' e terminam com '*/'.

''' css
/*.Basico.*/

/*.........................*/

  /*TAMBÉM PODE DESABILITAR PARTE DO CÓDIGO*/

# Anatomia
'''CSS

h1 {

    color: blue;

    front-side: 60px;

    Background: grey;

    }
'''
- Selector (seleciona o elemento)
- Declaration (dados a serem seguidos, cor, tamanho, fundo, etc)
- Properties (Propriedades)- Property Value (valores inseridos)


# Selector
- conecta elementos do HTML com o CSS p/ estilização
## Tipos:
- Global Selector '*'
- Element/Type selector h1,h2,p, div
- ID selector #box, #container
- Class selector .red, .m-4
- Atribute selector
- Pseudo Class
- Pseudo element
- Outros

HTML
<div id="container" class="m-40">
	<h1>Título</h1>
	<h2>Subtitulo</h2>
</div>

CSS
/* ID selector */
#container {
	width: 200px;
}

/* Class selector */
.m-40 {
	margin: 40px;
}

/* Element/Type selector + Agrupamento de seletores */
h1, h2 {

	color: blue;

	font-size: 60px;

	background: gray;

}

# Caixa
- Quase tudo são caixas
- Posicionamentos, tamanhos, espaçamentos, bordas, cores
- podem ficar uma ao lado da outra ou acima
- elementos html são caixas

border: xpx; /*borda*/

margin: xpx; /*esp fora*/

padding: xpx; /*esp dentro*/

# Adicionar CSS
## Inline
- Atributo 'style'
## style
- tag HTML que irá conter o CSS
## link
- arquivo css etxerno
## @import
- arquivo CSS externo