<h1>Projeto Interface Netflix</h1>

<p align="justify">Esse projeto faz parte do bootcamp "HTML Web Developer", disponibilizado pela Digital Innovation One. Nele aplico as principais tecnologias web:<b> HTML5, CSS3 e JavaScript</b>. 
Além disso, dentro do CSS3 apliquei técnicas com containers e variáveis, também utilizei o Flexbox para posicionar os elementos. A fim de implementar o carrossel de posters
de séries e filmes, manipulei plugins Jquery.</p>
<p>Dentro do <b>head</b> do HTML5 eu iniciei as importações dos documentos externos que serão indispensáveis para o projeto.</p>

<h2>Importações</h2>
<h3>Responsividade</h3>
<p>Sendo assim, importei o documento CSS que contém o código de responsividade da página web:</p>

	<link rel="stylesheet" href="style/responsividade.css">
	
<p align="justify">Nesse documento CSS de responsividade utilizei a regra <b>@media</b>, essa regra é empregada para definir estilos diferentes em mídias diferentes. O tipo de mídia chamada no documento é o <b>screen</b> 
que é usado para telas de computadores, tablets, celulares etc. Assim, para telas menores ou iguais a 700px, novas configurações foram aplicadas. A classe <b>container</b> dentro do header
tem a sua flex-direction alterada para <b>column</b>, ou seja, ela sai do modo linha e vai para o modo coluna. Desse modo, os links de navegação vão para baixo da logo Netflix. Além do mais,
a classe <b>botao</b> também sofre alteração com a diminuição da largura da tela, os botões filhos dessa classe ganham um nova altura e uma nova largura, além de uma margem superior.</p>
<p>Já para telas maiores ou iguais a 1000px de largura, a classe <b>descricaoo</b> começa a se ajustar a 50% do seu espaço.</p>

<h3>OWL CSS</h3>

<p align="justify">Para construir o carrossel de imagens de séries e filmes, utilizei o <a target="_blank" href="https://owlcarousel2.github.io/OwlCarousel2/">Owl Carousel 2</a>, que trata-se de um
plugin jQuery habilitado para o toque, permitindo a criação de sliders de carrossel responsivo.</p>
<p>Fiz o dowload do arquivo e utilizei alguns documentos de lá.</p>
<p>Arquivos na pasta <b>style</b>:</p>
<p>dist > assents > owl.carousel.min.css</p>

	<link rel="stylesheet" href="style/owl/owl.carousel.min.css">

<p>dist > assents > owl.theme.default.min.css</p>

	<link rel="stylesheet" href="style/owl/owl.theme.default.min.css">

<h3>OWL JS</h3>

<p>Arquivos na pasta <b>js</b>:</p>
<p>docs > assents > vendors > jquery.min</p>

	<script src="js/owl/jquery.min.js"></script>
	
<p>docs > assents > owlcarousel > owl.carousel.min.js</p>

	 <script src="js/owl/owl.carousel.min.js"></script>

<p align="justify">Neste documento <b>setup.js</b>, eu implementei o código JS que o próprio site do <a target="_blank" href="https://owlcarousel2.github.io/OwlCarousel2/">Owl Carousel 2</a>
indica. Trata-se de uma configuração básica, você pode encontrar ela <a target="_blank" href="https://owlcarousel2.github.io/OwlCarousel2/demos/basic.html">aqui</a>.</p>

	<script src="js/setup.js"></script>
	
<h3>Font Awesome</h3>

<p align="justify">O site <a target="_blank" href="https://fontawesome.com/">Font Awesome</a> permite encontrar diversos ícones gratuitos e pagos, ele disponibiliza esses ícones online e você
só precisa criar um cadastro e importar no seu arquivo HTML um script que será enviado para o e-mail cadastrado. Depois disso é só escolher o ícone que você deseja no site, copiar
o código que ele disponibiliza e colar no seu arquivo HTML. Eu utilizei no projeto os ícones de play e de informações, que estão dentro dos botões "ASSISTIR AGORA" e "MAIS INFORMAÇÕES",
respectivamente.</p>

<h2>Implementação</h2>

<h3>Header</h3>

<p align="justify"> Dentro da tag <b>header</b> eu implementei uma tag <b>div</b> com a classe <b>container</b>. A 'div .container' possui dois filhos, uma tag <b>h2</b> 
que contém o logo NETFLIX e uma tag <b>nav</b> que contém todos os links de navegação do site. A configuração CSS para a classe <b>container</b> dentro do header possui display
flex na sua configuração padrão, que é flex-direction: row. Além disso, alinhei esse container de forma centralizada em relação ao eixo y, com o align-items: center, e deixei os filhos dessa classe separados com o justify-content:
space-between.</p>

<h3>Main</h3>

<p align="justify">Dentro da tag <b>main</b> eu implementei uma tag <b>div</b> com a classe <b>filme-principal</b>. A 'div .filme-principal' possui dois filhos, uma tag <b>div</b>
com classe <b>container</b> e uma tag <b>div</b> com classe <b>botoes</b>. A configuração CSS para a classe <b>filme-principal</b> tem uma imagem como background e o seu display flex possui
flex-direction: column. Quando a flex-direction possui essa configuração o align-items fica referente ao eixo x e o justify-content fica referente ao eixo y.</p>

<h3>div class="carrossel-filmes"</h3>

<p align="justify">Dentro dessa div implementei o código HTML para o slider carrossel do plugin jQuery. Dentro de cada <b>div class="item"</b>, coloquei uma imagem com a classe
<b>box-filme</b>. A configuração CSS para cada imagem dentro dessa classe <b>box-filme</b> foi de largura 90% e altura 90%.</p>
