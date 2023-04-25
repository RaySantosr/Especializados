<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Produtos e Serviços - Descrição e Imagens</title>
</head>
<body>
  <h1>Produtos e Serviços</h1>
  <p>Descrição dos produtos e serviços aqui.</p>
  <img src="imagem2.jpg" alt="Imagem do produto ou serviço">
  <img src="imagem3.jpg" alt="Outra imagem do produto ou serviço">
  
  <h2>Mais Informações</h2>
  <form onsubmit="enviarMensagemWhatsapp(); return false;">
    <label for="email">Insira seu e-mail:</label>
    <input type="email" id="email" name="email" required>
    <br>
    <input type="submit" value="Enviar">
  </form>

  <script>
    function enviarMensagemWhatsapp() {
      var email = document.getElementById('email').value;
      var mensagem = 'Olá, gostaria de obter mais informações sobre o produto/serviço. Meu e-mail é ' + email;
      window.open('https://wa.me/5522999971204?text=' + encodeURIComponent(mensagem));
    }
  </script>
</body>
</html>
