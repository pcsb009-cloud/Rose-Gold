[paulinaysalome.html](https://github.com/user-attachments/files/23110023/paulinaysalome.html)
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>Rose Gold — Página Principal | Salome Bedoya, Paulina Correa</title>
  <style>
    body {
      background: linear-gradient(135deg, #FFD700, #E6A8D7);
      font-family: 'Poppins', sans-serif;
      text-align: center;
      color: #1a1a1a;
      margin: 0;
      padding: 0;
      min-height: 100vh;
    }
    h1 {
      color: #000;
      text-shadow: 2px 2px 6px rgba(255, 215, 0, 0.6);
      margin-top: 40px;
      font-size: 2.2em;
      letter-spacing: 1px;
    }
    nav {
      margin-top: 25px;
    }
    button {
      margin: 10px;
      text-decoration: none;
      color: #FFD700;
      background: #000;
      padding: 12px 25px;
      border-radius: 25px;
      font-weight: bold;
      font-size: 1em;
      border: none;
      cursor: pointer;
      box-shadow: 2px 2px 10px rgba(0, 0, 0, 0.4);
      transition: all 0.3s ease;
    }

    button:hover {
      background: #222;
      color: #fff;
      transform: scale(1.08);
      box-shadow: 0 0 15px rgba(255, 215, 0, 0.7);
    }

    .section {
      display: none;
      padding: 20px;
      margin-top: 30px;
      background: rgba(255, 255, 255, 0.9);
      border-radius: 20px;
      width: 90%;
      max-width: 1000px;
      margin-left: auto;
      margin-right: auto;
      box-shadow: 0 0 15px rgba(0, 0, 0, 0.3);
    }
    .active {
      display: block;
    }
    /* INFOGRAFÍA */
    .infografia {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
      gap: 25px;
      margin-top: 30px;
    }

    .producto {
      background: #fffaf0;
      border-radius: 15px;
      padding: 15px;
      box-shadow: 0 0 10px rgba(255, 215, 0, 0.4);
      transition: transform 0.3s ease, background 0.3s ease;
    }

    .producto:hover {
      transform: scale(1.05);
      background: #fff7e6;
    }
    .producto img {
      width: 110px;
      height: 110px;
      object-fit: cover;
      border-radius: 50%;
      margin-bottom: 10px;
      border: 3px solid #E6A8D7;
    }
    .producto h3 {
      margin: 10px 0 5px 0;
      color: #b36b00;
    }
    .producto p {
      font-size: 0.95em;
      color: #333;
    }
    .creditos {
      margin-top: 30px;
      font-weight: bold;
      color: #b36b00;
      font-size: 1.1em;
    }

    /* FORMULARIO */
    .form-container input, .form-container button {
      display: block;
      width: 80%;
      margin: 10px auto;
      padding: 10px;
      border-radius: 10px;
      border: 2px solid #FFD700;
      font-size: 1rem;
    }
    .form-container button {
      background: #000;
      color: #FFD700;
      font-weight: bold;
      cursor: pointer;
    }
    .form-container button:hover {
      background: #222;
      color: #fff;
    }
    /* SOPA DE LETRAS */
    .grid {
      display: grid;
      grid-template-columns: repeat(12, 35px);
      justify-content: center;
      gap: 5px;
      margin-top: 20px;
    }
    .cell {
      width: 35px;
      height: 35px;
      background: #fff0c4;
      border-radius: 6px;
      font-weight: bold;
      font-size: 18px;
      display: flex;
      align-items: center;
      justify-content: center;
      cursor: pointer;
      user-select: none;
    }
    .cell.selected {
      background: #FFD700;
      color: #000;
    }
    .cell.found {
      background: #000;
      color: #FFD700;
    }
    ul.words {
      list-style: none;
      padding: 0;
      margin-top: 15px;
      font-weight: bold;
    }
  </style>
</head>
<body>
  <h1>✨ Bienvenido a la página ROSE GOLD ✨</h1>
  <p>🌸 Explora nuestras secciones interactivas 🌸</p>
  <nav>
    <button onclick="mostrar('inicio')">Inicio</button>
    <button onclick="mostrar('juego')">Sopa de Letras</button>
    <button onclick="mostrar('formulario')">Formulario</button>
  </nav>
  <!-- SECCIÓN INICIO -->
  <div id="inicio" class="section active">
    <h2>🏠 Infografía de Productos de Oro</h2>
    <p>Descubre la elegancia y el brillo de nuestros productos exclusivos en oro y oro rosa. 💎</p>

    <div class="infografia">
      <div class="producto">
        <img src="https://www.eljineteazul.com/wp-content/uploads/2018/08/w1-17.jpg" alt="Anillo de oro">
        <h3>Anillos de Oro</h3>
        <p>Diseños modernos y clásicos hechos a mano con oro de 24 quilates. Perfectos para compromiso o estilo diario.</p>
      </div>
      <div class="producto">
        <img src="https://lcjoyeros.com/wp-content/uploads/2022/05/Sin-titulo-1.jpg" alt="Cadena de oro">
        <h3>Cadenas de Lujo</h3>
        <p>Cadenas finas, gruesas o entrelazadas, disponibles en oro amarillo y rosa, ideales para cualquier ocasión.</p>
      </div>
      <div class="producto">
        <img src="https://fabricadeoro.es/wp-content/uploads/2019/10/Pendientes-circonita-garra-presion-oro-chica.jpg" alt="Pendientes de oro">
        <h3>Aretes Sofisticados</h3>
        <p>Pendientes minimalistas y elegantes, con incrustaciones de piedras preciosas y detalles en oro rosa.</p>
      </div>
      <div class="producto">
        <img src="https://cdn-media.glamira.com/media/product/newgeneration/view/1/sku/fionnuala-4.5crt-m/diamond/ruby_AA/alloycolour/yellow.jpg" alt="Pulseras de oro">
        <h3>Pulseras Exclusivas</h3>
        <p>Pulseras trenzadas o lisas, con acabados de alta gama para combinar con cualquier outfit de lujo.</p>
      </div>
      <div class="producto">
        <img src="https://www.nomination.com/media/wysiwyg/News/IMG-INTERNE_BLOG-780x520_3__4.jpg" alt="Oro rosa">
        <h3>Colección Oro Rosa</h3>
        <p>Combinación perfecta entre elegancia y romanticismo. Nuestros tonos rosados son tendencia mundial.</p>
      </div>
      <div class="producto">
        <img src="https://static.wixstatic.com/media/226bff_1c98117ddd50488aba4208108c46fe4a~mv2.jpeg/v1/fill/w_498,h_498,al_c,q_80,usm_0.66_1.00_0.01,enc_avif,quality_auto/226bff_1c98117ddd50488aba4208108c46fe4a~mv2.jpeg" alt="Relojes de oro">
        <h3>Relojes Dorados</h3>
        <p>Relojes con mecanismos suizos y acabados en oro, diseñados para destacar tu presencia y elegancia.</p>
      </div>
      <div class="producto">
        <img src="https://static.wixstatic.com/media/45e2fd_6660a14b7b334d2eb1ec1af6a5a6b8b5~mv2.jpg/v1/fill/w_480,h_480,al_c,q_80,usm_0.66_1.00_0.01,enc_avif,quality_auto/45e2fd_6660a14b7b334d2eb1ec1af6a5a6b8b5~mv2.jpg" alt="Colgantes">
        <h3>Colgantes Personalizados</h3>
        <p>Personaliza tu inicial o símbolo especial en un colgante de oro macizo o rosa.</p>
      </div>
      <div class="producto">
        <img src="https://m.media-amazon.com/images/I/61OOPogV6jL._AC_UY1000_.jpg" alt="Sortijas">
        <h3>Sortijas de Lujo</h3>
        <p>Joyas finas con incrustaciones de diamantes naturales. Diseño exclusivo y artesanal.</p>
      </div>
    </div>
    <div class="creditos">Creado por: Salome Bedoya y Paulina Correa 💖</div>
  </div>
  <!-- SECCIÓN SOPA DE LETRAS -->
  <div id="juego" class="section">
    <h2>🍰 Sopa de Letras — Postres</h2>
    <p>Encuentra todos los postres escondidos en la cuadrícula.</p>
    <div id="board" class="grid"></div>
    <ul class="words" id="wordList"></ul>
  </div>
  <!-- SECCIÓN FORMULARIO -->
  <div id="formulario" class="section form-container">
    <h2>📝 Registro</h2>
    <form id="registerForm">
      <input type="text" id="nombre" name="nombre" placeholder="Nombre completo" required>
      <input type="email" id="email" name="email" placeholder="Correo electrónico" required>
      <input type="tel" id="telefono" name="telefono" placeholder="Teléfono (10 dígitos)" pattern="[0-9]{10}" required>
      <input type="password" id="password" name="password" placeholder="Contraseña" required>
      <input type="password" id="confirm" name="confirm" placeholder="Confirmar contraseña" required>
      <button type="submit">Registrarme</button>
    </form>
    <p id="successMsg" style="display:none; color:green; font-weight:bold;">¡Registro exitoso! 🎉</p>
  </div>

  <script>
    function mostrar(id) {
      document.querySelectorAll('.section').forEach(s => s.classList.remove('active'));
      document.getElementById(id).classList.add('active');
    }
    // Formulario
    document.getElementById('registerForm').addEventListener('submit', (e) => {
      e.preventDefault();
      const pass = document.getElementById('password').value;
      const conf = document.getElementById('confirm').value;
      if (pass !== conf) {
        alert('Las contraseñas no coinciden');
        return;
      }
      e.target.reset();
      document.getElementById('successMsg').style.display = 'block';
    });
    // Sopa de letras
    const words = ['TARTA','PASTEL','FLAN','COOKIE','DONUT','BROWNIE','HELADO','MOUSSE','CHURRO','PANNA'];
    const rows = 12, cols = 12;
    const boardEl = document.getElementById('board');
    const wordListEl = document.getElementById('wordList');
    let grid = Array.from({length: rows}, () => Array(cols).fill(''));
    const dirs = [[1,0],[-1,0],[0,1],[0,-1],[1,1],[-1,1],[1,-1],[-1,-1]];

    function colocarPalabras() {
      words.sort((a,b)=>b.length-a.length);
      for (const w of words) {
        for (let intento = 0; intento < 100; intento++) {
          const dir = dirs[Math.floor(Math.random()*dirs.length)];
          const [dx, dy] = dir;
          const x = Math.floor(Math.random()*cols);
          const y = Math.floor(Math.random()*rows);
          const endX = x + dx*(w.length-1);
          const endY = y + dy*(w.length-1);
          if (endX<0||endX>=cols||endY<0||endY>=rows) continue;
          let ok = true;
          for (let i=0;i<w.length;i++){
            const nx=x+dx*i, ny=y+dy*i;
            if(grid[ny][nx] && grid[ny][nx]!==w[i]) {ok=false;break;}
          }
          if(!ok) continue;
          for (let i=0;i<w.length;i++) grid[y+dy*i][x+dx*i]=w[i];
          break;
        }
      }
    }

    function rellenar() {
      const letras = 'ABCDEFGHIJKLMNOPQRSTUVWXYZ';
      for(let y=0;y<rows;y++) for(let x=0;x<cols;x++)
        if(!grid[y][x]) grid[y][x]=letras[Math.floor(Math.random()*letras.length)];
    }

    function renderizar() {
      boardEl.innerHTML = '';
      for(let y=0;y<rows;y++){
        for(let x=0;x<cols;x++){
          const div = document.createElement('div');
          div.className = 'cell';
          div.textContent = grid[y][x];
          div.dataset.x = x;
          div.dataset.y = y;
          boardEl.appendChild(div);
        }
      }
      wordListEl.innerHTML = words.map(w=>`<li>${w}</li>`).join('');
    }

    function iniciarJuego(){
      colocarPalabras();
      rellenar();
      renderizar();
    }

    iniciarJuego();
  </script>
</body>
</html>
