<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <title>Minha Jornada com HTML e CSS</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <!-- Google Fonts -->
  <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@700;900&display=swap" rel="stylesheet">

  <style>
    /* RESET */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Montserrat', sans-serif;
      min-height: 100vh;
      background: linear-gradient(270deg, #0f2027, #203a43, #2c5364);
      background-size: 600% 600%;
      animation: bgMove 12s ease infinite;
      color: #fff;
      overflow-x: hidden;
    }

    @keyframes bgMove {
      0% { background-position: 0% 50%; }
      50% { background-position: 100% 50%; }
      100% { background-position: 0% 50%; }
    }

    header {
      text-align: center;
      padding: 100px 20px;
    }

    h1 {
      font-size: 3.5rem;
      text-shadow: 0 0 10px #00f7ff, 0 0 20px #00f7ff;
      animation: glow 2s infinite alternate;
    }

    @keyframes glow {
      from {
        text-shadow: 0 0 10px #00f7ff;
      }
      to {
        text-shadow: 0 0 25px #00f7ff, 0 0 40px #00f7ff;
      }
    }

    header p {
      margin-top: 20px;
      font-size: 1.2rem;
      opacity: 0.9;
    }

    section {
      max-width: 1100px;
      margin: auto;
      padding: 80px 20px;
    }

    .card {
      background: rgba(255, 255, 255, 0.08);
      backdrop-filter: blur(10px);
      border-radius: 20px;
      padding: 40px;
      margin-bottom: 40px;
      box-shadow: 0 0 30px rgba(0, 247, 255, 0.2);
      transition: transform 0.4s, box-shadow 0.4s;
    }

    .card:hover {
      transform: translateY(-10px);
      box-shadow: 0 0 50px rgba(0, 247, 255, 0.5);
    }

    h2 {
      font-size: 2.2rem;
      margin-bottom: 20px;
      color: #00f7ff;
    }

    ul {
      list-style: none;
    }

    ul li {
      margin-bottom: 12px;
      position: relative;
      padding-left: 20px;
    }

    ul li::before {
      content: "▸";
      position: absolute;
      left: 0;
      color: #00f7ff;
    }

    .floating {
      animation: float 4s ease-in-out infinite;
      text-align: center;
      margin-top: 60px;
    }

    @keyframes float {
      0% { transform: translateY(0); }
      50% { transform: translateY(-15px); }
      100% { transform: translateY(0); }
    }

    footer {
      text-align: center;
      padding: 40px;
      opacity: 0.7;
      font-size: 0.9rem;
    }
  </style>
</head>

<body>

  <header>
    <h1>Minha Jornada com HTML e CSS</h1>
    <p>Aprendizado, evolução e o início de uma nova fase na tecnologia</p>
  </header>

  <section>
    <div class="card">
      <h2>Sobre o Projeto</h2>
      <p>
        Esta landing page foi criada para representar minha evolução no estudo
        de desenvolvimento web. Cada detalhe visual foi pensado para demonstrar
        organização, criatividade e boas práticas.
      </p>
    </div>

    <div class="card">
      <h2>O que aprendi</h2>
      <ul>
        <li>HTML semântico e bem estruturado</li>
        <li>CSS moderno com animações</li>
        <li>Layouts organizados</li>
        <li>Transições e efeitos visuais</li>
        <li>Experiência do usuário</li>
      </ul>
    </div>

    <div class="card floating">
      <h2>Este é só o começo</h2>
      <p>
        Continuarei estudando, praticando e evoluindo todos os dias.
      </p>
    </div>
  </section>

  <footer>
    Projeto desenvolvido com dedicação e foco no aprendizado
  </footer>

</body>
</html>
