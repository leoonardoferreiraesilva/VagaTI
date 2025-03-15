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
      font-size: 10vw; /* Fonte adaptável ao tamanho da largura da tela */
      margin: 0;
    }

    .header p {
      font-size: 5vw; /* Texto de contato adaptável */
      margin: 10px 0; /* Espaçamento responsivo */
    }

    .header a {
      color: yellow;
      text-decoration: none;
    }

    /* Container para as caixas de texto */
    .input-container {
      display: flex;
      flex-direction: column;
      gap: 10px; /* Espaçamento responsivo */
      width: 90%; /* Largura adaptável */
      max-width: 600px; /* Limite máximo para não ocupar telas muito grandes */
    }

    /* Estilos para as caixas de texto (textarea e input) */
    .input-container textarea,
    .input-container input {
      width: 100%; /* Adapta à largura do container */
      height: 80px; /* Altura fixa */
      background-color: transparent;
      border: 2px solid yellow;
      border-radius: 10px; /* Borda arredondada */
      color: white;
      font-size: 1rem; /* Tamanho de fonte relativo */
      padding: 10px;
      box-sizing: border-box;
      resize: none; /* Impede redimensionamento manual */
    }

    /* Estilos adaptáveis para diferentes telas */
    @media (max-width: 1920px) {
      body {
        background-color: black; /* Garante o fundo preto em telas menores */
      }

      .header h1 {
        font-size: 15vw; /* Fonte ainda maior em telas menores */
      }

      .header p {
        font-size: 6vw; /* Ajuste proporcional para telas médias */
      }

      .input-container textarea,
      .input-container input {
        height: 60px; /* Reduz a altura em telas menores */
      }
    }

    @media (max-width: 480px) {
      body {
        background-color: black; /* Fundo reforçado para telas pequenas */
      }

      .header p {
        font-size: 4.5vw; /* Reduz ainda mais o texto de contato */
      }

      .input-container textarea,
      .input-container input {
        height: 50px;
        font-size: 0.9rem; /* Ajuste de fonte em dispositivos muito pequenos */
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
    <!-- Caixa de texto 1 (textarea) para múltiplas linhas -->
    <textarea placeholder="Estagiário(a) Front-end ✨🚀
    Publicada em 15 de maio de 2024 https://tinyurl.com/29kmr7lz"></textarea>

    <!-- As demais caixas de texto -->
    <input type="text" placeholder="Caixa de texto 2">
    <input type="text" placeholder="Caixa de texto 3">
    <input type="text" placeholder="Caixa de texto 4">
    <input type="text" placeholder="Caixa de texto 5">
  </div>
</body>
</html>
