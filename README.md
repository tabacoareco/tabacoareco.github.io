
  <!-- Íconos FontAwesome -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

  <style>
    /* Configuración del fondo full screen */
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
      overflow: hidden; /* Evita barras de desplazamiento */
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
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
      pointer-events: none; /* Permite hacer clic en la imagen si no se toca un botón */
      transform: translateY(-50%);
      z-index: 10;
    }

    /* Estilo general de los botones */
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

    /* Adaptación para celulares */
    @media (max-width: 700px) {
      body {
        overflow: auto; /* Permite scroll solo en celulares si se acomodan verticalmente */
      }

      .side-buttons {
        position: relative;
        top: 0;
        transform: none;
        flex-direction: column;
        align-items: center;
        gap: 20px;
        margin-top: 60vh; /* Desplaza los botones abajo para lucir la ilustración en el cel */
        padding-bottom: 30px;
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

</body>
</html>
