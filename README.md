<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Vagas de TI</title>
  <link href="https://fonts.googleapis.com/css2?family=Pixelify+Sans&display=swap" rel="stylesheet">
  <style>
    /* Estilos gerais */
    html, body {
      margin: 0;
      padding: 0;
      width: 100%;
      height: 100%;
      background-color: black;
      color: white;
      font-family: 'Pixelify Sans', sans-serif;
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
      font-size: 10vw; /* Fonte adaptável ao tamanho da largura da tela */
      margin: 0;
    }

    .header p {
      font-size: 5vw; /* Texto de contato adaptável */
      margin: 10px 0;
    }

    .header a {
      color: yellow;
      text-decoration: none;
    }

    /* Container para as caixas de texto */
    .input-container {
      display: flex;
      flex-direction: column;
      gap: 10px;
      width: 90%;
      max-width: 600px;
    }

    /* Estilos para as caixas de texto (textarea e input) */
    .input-container textarea,
    .input-container input {
      width: 100%;
      height: 80px;
      background-color: transparent;
      border: 2px solid yellow;
      border-radius: 10px;
      color: white;
      font-size: 1rem;
      padding: 10px;
      box-sizing: border-box;
      resize: none;
    }

    /* Estilos adaptáveis para diferentes telas */
    @media (max-width: 768px) {
      .header h1 {
        font-size: 15vw; /* Fonte ainda maior em telas menores */
      }

      .header p {
        font-size: 6vw;
      }

      .input-container textarea,
      .input-container input {
        height: 60px;
      }
    }

    @media (max-width: 480px) {
      .header p {
        font-size: 4.5vw;
      }

      .input-container textarea,
      .input-container input {
        height: 50px;
        font-size: 0.9rem;
      }
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
    <textarea placeholder="Estagiário(a) Front-end ✨🚀
    Publicada em 15 de maio de 2024 https://tinyurl.com/29kmr7lz"></textarea>

    <input type="text" placeholder="Caixa de texto 2">
    <input type="text" placeholder="Caixa de texto 3">
    <input type="text" placeholder="Caixa de texto 4">
    <input type="text" placeholder="Caixa de texto 5">
  </div>
</body>
</html>
