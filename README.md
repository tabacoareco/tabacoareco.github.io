<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>TABACOS ARECO</title>
  
  <!-- Fuente de estilo tradicional / criollo -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,700;1,400&family=UnifrakturMaguntia&display=swap" rel="stylesheet">
  <!-- Ícono de WhatsApp -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

  <style>
    /* Fondo de pantalla usando únicamente la imagen fondo.jpg */
    body {
      background-image: url('fondo.jpg'); 
      background-size: cover;
      background-attachment: fixed;
      background-position: center;
      background-repeat: no-repeat;
      background-color: #1a1a1a;
      margin: 0;
      padding: 0;
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    }

    /* Tarjeta central semi-transparente para destacar los botones */
    .card {
      background-color: rgba(0, 0, 0, 0.75);
      backdrop-filter: blur(5px);
      border: 2px solid #c28d4b;
      padding: 40px 25px;
      border-radius: 16px;
      text-align: center;
      max-width: 450px;
      width: 85%;
      box-shadow: 0 10px 30px rgba(0, 0, 0, 0.8);
    }

    /* Título con estilo tradicional / criollo */
    h1 {
      font-family: 'UnifrakturMaguntia', 'Playfair Display', serif;
      color: #e0a96d;
      font-size: 3rem;
      margin: 0 0 10px 0;
      letter-spacing: 2px;
      text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.9);
    }

    /* Frase descriptiva */
    .slogan {
      color: #dddddd;
      font-family: 'Playfair Display', serif;
      font-style: italic;
      font-size: 1.1rem;
      margin-bottom: 30px;
      line-height: 1.4;
      border-bottom: 1px solid rgba(194, 141, 75, 0.5);
      padding-bottom: 20px;
    }

    /* Estilos de los botones */
    .btn {
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 10px;
      width: 100%;
      padding: 14px 0;
      margin-bottom: 15px;
      border-radius: 30px;
      text-decoration: none;
      font-weight: bold;
      font-size: 1.05rem;
      transition: all 0.3s ease;
      box-sizing: border-box;
    }

    /* Botón de la Lista de Precios PDF */
    .btn-pdf {
      background-color: #c28d4b;
      color: #ffffff;
      border: 1px solid #e0a96d;
    }

    .btn-pdf:hover {
      background-color: #a67335;
      transform: translateY(-2px);
      box-shadow: 0 5px 15px rgba(194, 141, 75, 0.4);
    }

    /* Botón de WhatsApp */
    .btn-whatsapp {
      background-color: #25d366;
      color: #ffffff;
    }

    .btn-whatsapp:hover {
      background-color: #1ebc57;
      transform: translateY(-2px);
      box-shadow: 0 5px 15px rgba(37, 211, 102, 0.4);
    }

    .footer {
      margin-top: 20px;
      font-size: 0.8rem;
      color: #aaaaaa;
    }
  </style>
</head>
<body>

  <div class="card">
    <h1>TABACOS ARECO</h1>
    <p class="slogan">"Para quienes saben apreciar el verdadero placer del tabaco."</p>

    <!-- Enlace al PDF con los precios -->
    <a href="index.pdf" target="_blank" class="btn btn-pdf">
      <i class="fa-solid fa-file-pdf"></i> Ver Lista de Precios
    </a>

    <!-- Enlace directo a WhatsApp con tu número -->
    <a href="https://wa.me/5492325404049" target="_blank" class="btn btn-whatsapp">
      <i class="fa-brands fa-whatsapp fa-lg"></i> Consultar por WhatsApp
    </a>

    <div class="footer">
      <p>San Antonio de Areco, Argentina</p>
    </div>
  </div>

</body>
</html>
