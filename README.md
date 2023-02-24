<h1>Recomendação de Produtos por Similaridade</h1> 
<br>
<div align='justify'>
	<p>Um sistema simple de recomendação baseados na aparência do produto. Para um dado produto, obtém-se uma quantidade pré-definida de outros produtos similares</p>
	<p>É um sistema parecido com essas que vêmos em buscadores ou em mídias sociais.</p> 
	<p>À partir do que fazemos uma perquisa o sistema nos mostra também podutos similares que talvez sejam de nosso interesse.</p>
	<p>Para isso foi usado uma modelo CNN (Rede Neural Convolucional) pré-treinado do Keras para extrair features das imagens. Então são calculadas as similaridades entre produtos.</p>
	<p>Nesse projeto foi usado o modelo VGG16 do <a href='https://www.image-net.org/'>imagenet</a>.</p>
	<p>Para não usar todo o modelo e recuperar apenas as informações que ele foi capaz de retirar das imagens, foi removida a última camada que é usada apenas 
para predição de classe.</p>

</div>
<div>
	<p>O passo a passo:</p>
	<ol>
		<li>Imports e setup dos parâmetros</li>
		<li>Carregar o modelo VGG pre-traineda do Keras</li>
		<li>Pegar o caminho das imagens
		<li>Inserir uma imagem no CNN (Rede Neural Convolucional)</li>
		<li>Alimentar a CNN com todas as imagens</li>
		<li>Calcular o cosseno das similaridades</li>
		<li>Através de uma função, encontrar os produtos mais similares</li>
   </ol>
</div>
