<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Tabacos Areco</title>
  
  <!-- Fuente tradicional de gran legibilidad -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@1,700;1,900&display=swap" rel="stylesheet">
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

    /* Ubicación de la leyenda en la parte superior */
    .top-slogan-box {
      margin-top: 30px;
      text-align: center;
      max-width: 90%;
      padding: 0 10px;
    }

    /* Frase en letra negra destacada */
    .slogan {
      color: #000000;
      font-family: 'Playfair Display', serif;
      font-style: italic;
      font-weight: 900;
      font-size: 1.5rem;
      margin: 0;
      line-height: 1.3;
      letter-spacing: 0.5px;
      text-shadow: 0px 1px 2px rgba(255, 255, 255, 0.6), 0px -1px 2px rgba(255, 255, 255, 0.6);
    }

    /* Contenedor flotante para los botones laterales */
    .side-buttons {
      position: fixed;
      top: 50%;
      left: 0;
      width: 100%;
      display: flex;
      justify-content: space-between;
      padding: 0 30px;
      box-sizing: border-box;
      pointer-events: none;
      transform: translateY(-50%);
      z-index: 10;
    }

    /* Estilo de los botones */
    .btn-side {
      pointer-events: auto;
      display: flex;
      align-items: center;
      gap: 12px;
      padding: 16px 26px;
      border-radius: 50px;
      text-decoration: none;
      font-weight: bold;
      font-size: 1.05rem;
      box-shadow: 0 8px 20px rgba(0, 0, 0, 0.6);
      transition: all 0.3s ease;
    }

    /* Botón Izquierdo - PDF Lista de precios */
    .btn-pdf {
      background-color: rgba(194, 141, 75, 0.95);
      color: #ffffff;
      border: 1px solid #e0a96d;
    }

    .btn-pdf:hover {
      background-color: #c28d4b;
      transform: scale(1.08) translateX(5px);
    }

    /* Botón Derecho - WhatsApp */
    .btn-whatsapp {
      background-color: rgba(37, 211, 102, 0.95);
      color: #ffffff;
      border: 1px solid #20ba5a;
    }

    .btn-whatsapp:hover {
      background-color: #25d366;
      transform: scale(1.08) translateX(-5px);
    }

    /* Pie de página discreto */
    .footer {
      margin-bottom: 15px;
      font-size: 0.85rem;
      color: #000000;
      font-weight: bold;
      text-shadow: 0px 1px 2px rgba(255, 255, 255, 0.6);
    }

    /* Ajuste para celulares */
    @media (max-width: 700px) {
      .slogan {
        font-size: 1.2rem;
      }

      .top-slogan-box {
        margin-top: 20px;
      }

      .side-buttons {
        position: relative;
        top: 0;
        transform: none;
        flex-direction: column;
        align-items: center;
        gap: 15px;
        margin: 25px 0;
      }

      .btn-side {
        width: 85%;
        justify-content: center;
      }
    }
  </style>
</head>
<body>

 

  <!-- Botones Ubicados a los Laterales -->
  <div class="side-buttons">
    <!-- Izquierda: Lista en PDF -->
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
