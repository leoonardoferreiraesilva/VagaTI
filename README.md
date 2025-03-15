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
      margin: 5px 0 20px;
    }
    
    .header a {
      color: yellow;
      text-decoration: none;
    }
    
    /* Container para as caixas de texto */
    .input-container {
      display: flex;
      flex-direction: column;
      gap: 5px;
    }
    
    /* Estilos para as caixas de texto (textarea e input) */
    .input-container textarea,
    .input-container input {
      width: 1500px;
      height: 100px;
      background-color: transparent;
      border: 2px solid yellow;
      border-radius: 10px;
      color: white;
      font-size: 22px;
      padding: 5px;
      box-sizing: border-box;
      resize: none;
    }

    /* Estilo para os links criados automaticamente */
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
    <textarea class="auto-link" placeholder="Estagiário(a) Front-end ✨🚀
    Publicada em 15 de maio de 2024 https://tinyurl.com/29kmr7lz"></textarea>
    
    <!-- As demais caixas, utilizando input para linha única -->
    <input class="auto-link" type="text" placeholder="Caixa de texto 2 com https://example.com">
    <input class="auto-link" type="text" placeholder="Caixa de texto 3">
    <input class="auto-link" type="text" placeholder="Caixa de texto 4">
    <input class="auto-link" type="text" placeholder="Caixa de texto 5">
  </div>
    
  <!-- Script para converter URLs em links clicáveis -->
  <script>
    function linkify(text) {
      // Expressão regular para encontrar URLs
      const urlPattern = /(\b(https?|ftp):\/\/[-A-Z0-9+&@#\/%?=~_|!:,.;]*[-A-Z0-9+&@#\/%=~_|])/gi;
      return text.replace(urlPattern, function(match) {
        return '<a class="auto-generated" href="' + match + '" target="_blank">' + match + '</a>';
      });
    }

    // Converte texto em links clicáveis automaticamente
    document.addEventListener('DOMContentLoaded', function() {
      const inputs = document.querySelectorAll('.auto-link');
      inputs.forEach((input) => {
        input.addEventListener('blur', function () {
          const value = input.value;
          if (value) {
            input.outerHTML = linkify(value);
          }
        });
      });
    });
  </script>
</body>
</html>
