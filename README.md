<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Oliveira Store</title>
  <!-- Bootstrap -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
  <style>
    body {
      font-family: Arial, sans-serif;
    }
    .navbar-brand img {
      height: 50px;
    }
    .carousel-item img {
      max-height: 500px;
      object-fit: cover;
    }
    .card img {
      max-height: 250px;
      object-fit: cover;
    }
  </style>
</head>
<body>

  <!-- Navbar -->
  <nav class="navbar navbar-expand-lg navbar-dark bg-dark shadow">
    <div class="container">
      <a class="navbar-brand" href="#">
        <img src="OliveiraStore..jpg" alt="Logo Oliveira Store">
      </a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav ms-auto">
          <li class="nav-item"><a class="nav-link" href="#welcome">Início</a></li>
          <li class="nav-item"><a class="nav-link" href="#products">Produtos</a></li>
          <li class="nav-item"><a class="nav-link" href="https://wa.me/5516993082820" target="_blank">Contato</a></li>
          <li class="nav-item"><a class="nav-link" href="https://www.instagram.com/oliveira_store27" target="_blank">Instagram</a></li>
          <li class="nav-item"><a class="nav-link" data-bs-toggle="modal" data-bs-target="#sobreModal">Sobre Nós</a></li>
        </ul>
      </div>
    </div>
  </nav>

  <!-- Tela de boas-vindas -->
  <section id="welcome" class="text-center py-5 bg-light">
    <div class="container">
      <h1 class="display-5 fw-bold mb-3">Bem-vindo à Oliveira Store!</h1>
      <p class="lead mb-4">Estilo, qualidade e preço justo em um só lugar.</p>
      <a href="#products" class="btn btn-warning btn-lg fw-bold">Ver Produtos</a>
    </div>
  </section>

  <!-- Produtos -->
  <section id="products" class="container py-5">
    <h2 class="text-center mb-5">Nossos Produtos</h2>

    <!-- Carrossel -->
    <div id="produtosCarousel" class="carousel slide mb-5" data-bs-ride="carousel">
      <div class="carousel-inner">

        <div class="carousel-item active">
          <img src="Kit.png" class="d-block w-100" alt="Kit Bermuda/Camisa">
          <div class="carousel-caption d-none d-md-block bg-dark bg-opacity-50 rounded">
            <h5>Kit Bermuda/Camisa</h5>
            <p>R$ 140,00</p>
            <a href="https://wa.me/5516993082820?text=Olá,%20quero%20o%20Kit%20Bermuda%2FCamisa" class="btn btn-warning">Comprar</a>
          </div>
        </div>

        <div class="carousel-item">
          <img src="Kit2.png" class="d-block w-100" alt="Camisa Premium">
          <div class="carousel-caption d-none d-md-block bg-dark bg-opacity-50 rounded">
            <h5>Camisa Premium</h5>
            <p>R$ 89,90</p>
            <a href="https://wa.me/5516993082820?text=Olá,%20quero%20a%20Camisa%20Premium" class="btn btn-warning">Comprar</a>
          </div>
        </div>

        <div class="carousel-item">
          <img src="bermuda.png" class="d-block w-100" alt="Bermuda Jeans">
          <div class="carousel-caption d-none d-md-block bg-dark bg-opacity-50 rounded">
            <h5>Bermuda Jeans</h5>
            <p>R$ 120,00</p>
            <a href="https://wa.me/5516993082820?text=Olá,%20quero%20a%20Bermuda%20Jeans" class="btn btn-warning">Comprar</a>
          </div>
        </div>

      </div>
      <button class="carousel-control-prev" type="button" data-bs-target="#produtosCarousel" data-bs-slide="prev">
        <span class="carousel-control-prev-icon"></span>
      </button>
      <button class="carousel-control-next" type="button" data-bs-target="#produtosCarousel" data-bs-slide="next">
        <span class="carousel-control-next-icon"></span>
      </button>
    </div>

    <!-- Grade de Cards -->
    <div class="row row-cols-1 row-cols-md-3 g-4">
      <div class="col">
        <div class="card h-100 shadow-sm">
          <img src="Kit.png" class="card-img-top" alt="Kit Bermuda/Camisa">
          <div class="card-body text-center">
            <h5 class="card-title">Kit Bermuda/Camisa</h5>
            <p class="text-warning fw-bold">R$ 140,00</p>
            <a href="https://wa.me/5516993082820?text=Olá,%20quero%20o%20Kit%20Bermuda%2FCamisa" target="_blank" class="btn btn-warning fw-bold">Comprar</a>
          </div>
        </div>
      </div>
      <div class="col">
        <div class="card h-100 shadow-sm">
          <img src="Driftit.png" class="card-img-top" alt="Camisa Premium">
          <div class="card-body text-center">
            <h5 class="card-title">Camisa Premium</h5>
            <p class="text-warning fw-bold">R$ 89,90</p>
            <a href="https://wa.me/5516993082820?text=Olá,%20quero%20a%20Camisa%20Premium" target="_blank" class="btn btn-warning fw-bold">Comprar</a>
          </div>
        </div>
      </div>
      <div class="col">
        <div class="card h-100 shadow-sm">
          <img src="Bermudas.png" class="card-img-top" alt="Bermuda Jeans">
          <div class="card-body text-center">
            <h5 class="card-title">Bermuda Jeans</h5>
            <p class="text-warning fw-bold">R$ 120,00</p>
            <a href="https://wa.me/5516993082820?text=Olá,%20quero%20a%20Bermuda%20Jeans" target="_blank" class="btn btn-warning fw-bold">Comprar</a>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Modal Sobre Nós -->
  <div class="modal fade" id="sobreModal" tabindex="-1">
    <div class="modal-dialog modal-lg modal-dialog-centered">
      <div class="modal-content">
        <div class="modal-header">
          <h5 class="modal-title">Sobre Nós</h5>
          <button type="button" class="btn-close" data-bs-dismiss="modal"></button>
        </div>
        <div class="modal-body text-center">
          <img src="Sobre.png" alt="Sobre Nós" class="img-fluid rounded mb-3">
          <p>Somos a Oliveira Store, referência em moda. Qualidade, estilo e atendimento de primeira.</p>
        </div>
      </div>
    </div>
  </div>

  <!-- Bootstrap JS -->
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
