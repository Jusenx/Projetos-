<!doctype html>
<html lang="pt-BR">
<head>
	<meta charset="utf-8">
	<title>Requisição XMLHttpRequest</title>
    
</head>
<body>
	<h1>Imagens Aleatórios de Cachorros</h1>
	<p>A partir do click no botão abaixo uma nova imagem aleatória de cachorros será carregada utilizando requisições assíncronas com XMLHttpRequest</p>

	<img id="img_dog" src="" alt="Aguardando a imagem ser carregada" />
	<br/>
	<button onclick="carregarImagens()">Carregar Imagens</button>
    
    <p>Segunda Tentativa de Criar uma Imagem Aleatoria</p>

    <img id="img_alt" src="" alt="espere a imagem carregar" /> 
    <br/>
    <button onclick="imagemaleatoria()">Imagem Aleatoria</button>

</body>
	<script type="text/javascript">
    
	
		function carregarImagens(){
            
		
			var url = "https://dog.ceo/api/breeds/image/random"
			fetch(url, {
				method: 'get'
			})
			.then(function(response) {
				response.json().then(function(data){
					console.log('Resultado da Requisição: ' + data.message);

					var imgDog = document.getElementById("img_dog");
					imgDog.src = data.message;
				});
			})
			.catch(function(err) {
				console.error('O seguinte erro ocorreu durante a requisição: ' + err);
			});

		}

        function imagemaleatoria(){
		
        var url = "https://dog.ceo/api/breeds/image/random"
        fetch(url, {
            method: 'get'
        })
        .then(function(response) {
            response.json().then(function(data){
                console.log('Resultado da Requisição: ' + data.message);

                var imgAlt = document.getElementById("img_alt");
                imgAlt.src = data.message;
            });
        })
        .catch(function(err) {
            console.error('O seguinte erro ocorreu durante a requisição: ' + err);
        });

    }
	</script>
</html>
