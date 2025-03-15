<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Vagas de TI</title>
  <link href="https://fonts.googleapis.com/css2?family=Pixelify+Sans&display=swap" rel="stylesheet">
  <style>
    /* Estilos gerais */
    body {
      background-color: black;
      color: white;
      font-family: 'Pixelify Sans', sans-serif;
      margin: 0;
      padding: 20px;
      display: flex;
      flex-direction: column;
      align-items: center;
    }
    
    /* Seção superior: Título e Contato */
    .header {
      text-align: center;
      margin-bottom: 20px;
    }
    
    .header h1 {
      font-size: 128px;
      margin: 0;
    }
    
    .header p {
      font-size: 80px;
      margin: 5px 0 20px; /* 5px de espaço entre o título e o texto de contato */
    }
    
    .header a {
      color: yellow;
      text-decoration: none;
    }
    
    /* Container para as caixas de texto */
    .input-container {
      display: flex;
      flex-direction: column;
      gap: 5px; /* 5px de espaçamento entre as caixas */
    }
    
    /* Estilos para as caixas de texto (textarea e input) */
    .input-container textarea,
    .input-container input {
      width: 1500px;           /* Ajuste de largura conforme desejado */
      height: 100px;           /* Ajuste de altura conforme desejado */
      background-color: transparent;
      border: 2px solid yellow;
      border-radius: 10px;      /* Borda arredondada */
      color: white;
      font-size: 22px;
      padding: 5px;
      box-sizing: border-box;
      resize: none;           /* Impede redimensionamento manual */
    }
    
    /* (Opcional) Estilo para links gerados automaticamente */
    a.auto-generated {
      color: yellow;
      text-decoration: underline;
    }
  </style>
</head>
<body>
  <div class="header">
    <h1>VAGAS de TI</h1>
    <p>
      CONTATO: 
      <a href="https://linkedin.com/in/leonardoferreiraesilva/" target="_blank">
        linkedin.com/in/leonardoferreiraesilva/
      </a>
    </p>
  </div>
  
  <div class="input-container">
    <!-- Caixa de texto 1 (textarea) para múltiplas linhas -->
    <textarea placeholder="Estagiário(a) Front-end ✨🚀
    Publicada em 15 de maio de 2024 https://tinyurl.com/29kmr7lz"></textarea>
    
    <!-- As demais caixas, utilizando input para linha única -->
    <input type="text" placeholder="Caixa de testo2"></textarea>
    <input type="text" placeholder="Caixa de texto 3"></textarea>
    <input type="text" placeholder="Caixa de texto 4"></textarea>
    <input type="text" placeholder="Caixa de texto 5"></textarea>
  </div>
    
  <!-- Script para converter URLs em links clicáveis -->
  <script>
    function linkify(text) {
      // Expressão regular para encontrar URLs que começam com http://, https:// ou ftp://
      var urlPattern = /(\b(https?|ftp):\/\/[-A-Z0-9+&@#\/%?=~_|!:,.;]*[-A-Z0-9+&@#\/%=~_|])/ig;
      return text.replace(urlPattern, function(match) {
        return '<a class="auto-generated" href="' + match + '" target="_blank">' + match + '</a>';
      });
    }
    
    // Aplica a função linkify aos elementos com a classe "auto-link"
    document.addEventListener('DOMContentLoaded', function() {
      var elements = document.getElementsByClassName('auto-link');
      for (var i = 0; i < elements.length; i++) {
        var el = elements[i];
        // Converte o texto interno (innerText) em HTML com links clicáveis.
        el.innerHTML = linkify(el.innerText);
      }
    });
  </script>
</body>
</html>
