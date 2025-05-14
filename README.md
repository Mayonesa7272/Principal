<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Mi Portafolio</title>
  <style>
    body {
      font-family: 'Segoe UI', sans-serif;
      margin: 0;
      background-color: #f4f4f4;
      color: #333;
    }

    header {
      background-color: #282c34;
      color: white;
      text-align: center;
      padding: 2em 1em;
    }

    h1 {
      margin-bottom: 0.2em;
    }

    .container {
      max-width: 900px;
      margin: 2em auto;
      padding: 0 1em;
    }

    .accordion {
      background-color: #fff;
      color: #444;
      cursor: pointer;
      padding: 1em;
      width: 100%;
      border: none;
      text-align: left;
      outline: none;
      font-size: 1.1em;
      transition: background-color 0.3s ease;
      margin-bottom: 0.5em;
      border-radius: 5px;
      box-shadow: 0 2px 4px rgba(0,0,0,0.1);
    }

    .accordion:hover {
      background-color: #e0e0e0;
    }

    .panel {
      padding: 0 1em;
      background-color: white;
      display: none;
      overflow: hidden;
      border-radius: 0 0 5px 5px;
      border-left: 2px solid #007acc;
      border-right: 2px solid #007acc;
      border-bottom: 2px solid #007acc;
    }

    .panel ul {
      padding-left: 1.2em;
    }

    footer {
      text-align: center;
      padding: 1em;
      background-color: #282c34;
      color: white;
      margin-top: 2em;
    }
  </style>
</head>
<body>

  <header>
    <h1>Mi Portafolio</h1>
    <p>Desarrollador Web & Creativo Digital</p>
  </header>

  <div class="container">
    <button class="accordion">💻 Programas</button>
    <div class="panel">
      <ul>
        <li>Editor de texto personalizado en Python</li>
        <li>Gestor de tareas con base de datos SQLite</li>
        <li>App de finanzas personales (Electron + JS)</li>
      </ul>
    </div>

    <button class="accordion">🌐 Páginas Web</button>
    <div class="panel">
      <ul>
        <li><a href="https://miportafolio.github.io">Portafolio Personal</a></li>
        <li><a href="https://proyecto-tienda.github.io">Tienda Online (simulada)</a></li>
        <li><a href="https://climaapp.github.io">App del Clima</a></li>
      </ul>
    </div>

    <button class="accordion">🔗 Enlaces Externos</button>
    <div class="panel">
      <ul>
        <li><a href="https://github.com/tuusuario" target="_blank">Mi GitHub</a></li>
        <li><a href="https://linkedin.com/in/tuusuario" target="_blank">LinkedIn</a></li>
        <li><a href="mailto:tuemail@ejemplo.com">Correo Electrónico</a></li>
      </ul>
    </div>

    <button class="accordion">📁 Recursos</button>
    <div class="panel">
      <ul>
        <li><a href="#">Plantillas HTML gratuitas</a></li>
        <li><a href="#">Bibliotecas de iconos</a></li>
        <li><a href="#">Cursos y tutoriales</a></li>
      </ul>
    </div>

    <button class="accordion">📜 Sobre mí</button>
    <div class="panel">
      <p>Soy un desarrollador en formación apasionado por la web, la programación creativa y el diseño limpio. Me encanta aprender nuevas tecnologías y colaborar en proyectos interesantes.</p>
    </div>
  </div>

  <footer>
    &copy; 2025 - Mi Nombre | Hecho con ❤️ usando GitHub Pages
  </footer>

  <script>
    const accordions = document.querySelectorAll(".accordion");
    accordions.forEach(btn => {
      btn.addEventListener("click", function () {
        this.classList.toggle("active");
        const panel = this.nextElementSibling;
        if (panel.style.display === "block") {
          panel.style.display = "none";
        } else {
          panel.style.display = "block";
        }
      });
    });
  </script>

</body>
</html>
