<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>TABACOS ARECO</title>
  
  <!-- Fuentes tradicionales -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,700;1,400&family=UnifrakturMaguntia&display=swap" rel="stylesheet">
  <!-- Íconos FontAwesome -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

  <style>
    /* Configuración del fondo */
    body {
      background-image: url('fondo.jpg'); 
      background-size: cover;
      background-attachment: fixed;
      background-position: center;
      background-repeat: no-repeat;
      background-color: #1a1a1a;
      margin: 0;
      padding: 0;
      min-height: 100vh;
      box-sizing: border-box;
      display: flex;
      flex-direction: column;
      justify-content: space-between;
      align-items: center;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    }

    /* Encabezado superior transparente */
    .header-box {
      margin-top: 30px;
      background-color: rgba(0, 0, 0, 0.75);
      backdrop-filter: blur(4px);
      border: 1px solid rgba(194, 141, 75, 0.6);
      padding: 20px 30px;
      border-radius: 12px;
      text-align: center;
      max-width: 90%;
      box-shadow: 0 8px 25px rgba(0, 0, 0, 0.8);
    }

    h1 {
      font-family: 'UnifrakturMaguntia', 'Playfair Display', serif;
      color: #e0a96d;
      font-size: 2.8rem;
      margin: 0 0 5px 0;
      letter-spacing: 2px;
      text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.9);
    }

    .slogan {
      color: #e0e0e0;
      font-family: 'Playfair Display', serif;
      font-style: italic;
      font-size: 1.05rem;
      margin: 0;
    }

    /* Contenedor flotante para los laterales */
    .side-buttons {
      position: fixed;
      top: 55%;
      left: 0;
      width: 100%;
      display: flex;
      justify-content: space-between;
      padding: 0 25px;
      box-sizing: border-box;
      pointer-events: none; /* Permite hacer clic en el fondo */
      transform: translateY(-50%);
      z-index: 10;
    }

    /* Estilo general de los botones laterales */
    .btn-side {
      pointer-events: auto; /* Activa la interacción del clic */
      display: flex;
      align-items: center;
      gap: 12px;
      padding: 16px 24px;
      border-radius: 50px;
      text-decoration: none;
      font-weight: bold;
      font-size: 1rem;
      box-shadow: 0 6px 20px rgba(0, 0, 0, 0.6);
      transition: all 0.3s ease;
      backdrop-filter: blur(2px);
    }

    /* Botón Lateral Izquierdo - PDF */
    .btn-pdf {
      background-color: rgba(194, 141, 75, 0.92);
      color: #ffffff;
      border: 1px solid #e0a96d;
    }

    .btn-pdf:hover {
      background-color: #c28d4b;
      transform: scale(1.08) translateX(5px);
    }

    /* Botón Lateral Derecho - WhatsApp */
    .btn-whatsapp {
      background-color: rgba(37, 211, 102, 0.92);
      color: #ffffff;
      border: 1px solid #20ba5a;
    }

    .btn-whatsapp:hover {
      background-color: #25d366;
      transform: scale(1.08) translateX(-5px);
    }

    /* Pie de página */
    .footer {
      margin-bottom: 20px;
      background-color: rgba(0, 0, 0, 0.6);
      padding: 6px 16px;
      border-radius: 20px;
      font-size: 0.8rem;
      color: #cccccc;
    }

    /* Adaptación para pantallas de celulares pequeños */
    @media (max-width: 650px) {
      .side-buttons {
        position: relative;
        top: 0;
        transform: none;
        flex-direction: column;
        align-items: center;
        gap: 15px;
        margin: 40px 0;
      }

      .btn-side {
        width: 80%;
        justify-content: center;
      }

      h1 {
        font-size: 2.1rem;
      }
    }
  </style>
</head>
<body>

  <!-- Encabezado Superior -->
  <div class="header-box">
    <h1>TABACOS ARECO</h1>
    <p class="slogan">"Para quienes saben apreciar el verdadero placer del tabaco."</p>
  </div>

  <!-- Botones Ubicados a los Laterales -->
  <div class="side-buttons">
    <!-- Izquierda: PDF -->
    <a href="index.pdf" target="_blank" class="btn-side btn-pdf">
      <i class="fa-solid fa-file-pdf fa-lg"></i> Lista de Precios
    </a>

    <!-- Derecha: WhatsApp -->
    <a href="https://wa.me/5492325404049" target="_blank" class="btn-side btn-whatsapp">
      <i class="fa-brands fa-whatsapp fa-xl"></i> WhatsApp
    </a>
  </div>

  <!-- Pie de Página -->
  <div class="footer">
    San Antonio de Areco, Argentina
  </div>

</body>
</html>
