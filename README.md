<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>ARABE7</title>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Rubik+Glitch&display=swap');

    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: Arial, sans-serif;
      background-color: #000;
      color: white;
      text-align: center;
      overflow-x: hidden;
    }

    .fade-in {
      opacity: 0;
      transform: translateY(20px);
      transition: all 0.6s ease;
    }

    .fade-in.visible {
      opacity: 1;
      transform: translateY(0);
    }

    @keyframes shakeFade {
      0% { opacity: 0; transform: translate(0, 0); }
      25% { transform: translate(2px, -2px); }
      50% { transform: translate(-2px, 2px); }
      75% { transform: translate(2px, 2px); }
      100% { opacity: 1; transform: translate(0, 0); }
    }

    @keyframes gradientText {
      0% { background-position: 0% 50%; }
      100% { background-position: 100% 50%; }
    }

    .hidden {
      display: none !important;
      pointer-events: none;
    }

    .header-img {
      width: 100%;
      max-height: 200px;
      object-fit: cover;
    }

    .profile-pic {
      width: 120px;
      height: 120px;
      border-radius: 50%;
      margin-top: -60px;
      border: 3px solid #000;
      cursor: pointer;
    }

    h1 {
      font-size: 28px;
      margin: 10px 0;
      font-family: 'Rubik Glitch', cursive;
    }

    .phone {
      margin: 10px 0;
      font-size: 18px;
      color: #aaa;
      cursor: pointer;
    }

    .buttons {
      display: flex;
      justify-content: center;
      gap: 20px;
      margin-top: 20px;
      flex-wrap: wrap;
    }

    .button {
      background-color: #111;
      border: 1px solid #333;
      border-radius: 10px;
      padding: 15px 20px;
      color: white;
      text-decoration: none;
      font-weight: bold;
      transition: 0.3s;
      display: flex;
      align-items: center;
      gap: 10px;
    }

    .button:hover {
      background-color: #222;
    }

    .button img {
      width: 30px;
      height: 30px;
      border-radius: 5px;
    }

    .status {
      color: #00ff00;
      margin-top: 20px;
    }

    .quote {
      margin-top: 10px;
      font-size: 14px;
      color: #ccc;
    }

    .info-boxes {
      margin-top: 30px;
      padding: 0 20px;
    }

    .info-box {
      background-color: #111;
      border: 1px solid #333;
      border-radius: 10px;
      padding: 15px;
      margin-bottom: 20px;
      text-align: left;
    }

    .info-box h2 {
      margin-top: 0;
      background: linear-gradient(270deg, #00ff00, #000);
      background-size: 400% 400%;
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      animation: gradientText 5s ease infinite;
      text-transform: uppercase;
      font-family: 'Rubik Glitch', cursive;
    }

    .info-box p {
      color: #ccc;
    }

    #fullscreen {
      display: none;
      position: fixed;
      top: 0; left: 0;
      width: 100vw;
      height: 100vh;
      background-color: rgba(0, 0, 0, 0.95);
      justify-content: center;
      align-items: center;
      z-index: 9999;
    }

    #fullscreen img {
      max-width: 90%;
      max-height: 90%;
      border-radius: 20px;
      animation: zoomIn 0.5s ease;
    }

    @keyframes zoomIn {
      from { transform: scale(0.5); opacity: 0; }
      to { transform: scale(1); opacity: 1; }
    }
  .products {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 20px;
  margin-top: 30px;
}

.product {
  background-color: #111;
  border: 1px solid #333;
  border-radius: 10px;
  padding: 20px;
  text-align: center;
  transition: transform 0.3s ease;
}

.product img {
  width: 100%;
  height: auto;
  border-radius: 10px;
}

.product h3 {
  font-size: 18px;
  color: #fff;
  margin: 10px 0;
  font-family: 'Rubik Glitch', cursive;
}

.product p {
  color: #ccc;
  font-size: 14px;
  margin-bottom: 15px;
}

.product a {
  display: inline-block;
  background-color: #00ff00;
  color: white;
  text-decoration: none;
  padding: 10px 20px;
  border-radius: 10px;
  font-weight: bold;
  transition: background-color 0.3s ease;
}

.product a:hover {
  background-color: #00cc00;
}

.product:hover {
  transform: translateY(-10px);
}
  </style>
</head>
<body>
  <img class="header-img fade-in" src="https://i.imgur.com/C6bKcXC.jpeg" alt="Header">
  <img class="profile-pic fade-in" src="https://i.imgur.com/qv2zzf3.jpeg" alt="Profile" onclick="showFullscreen()">

  <h1 class="fade-in">A R A B E7</h1>
  <div class="phone fade-in" onclick="copyPhone()">+55 13 98193-5658</div>

  <div class="buttons fade-in">
    <a class="button" href="tel:+5513981935658">
      <img src="https://i.imgur.com/HyicXGC.jpeg" alt="Contato">
      CONTATO
    </a>
    <a class="button" href="https://whatsapp.com/channel/0029VbA1TggBvvskwsWyX221" target="_blank">
      <img src="https://i.imgur.com/cxfb6C1.png" alt="Divine">
      DIVINE
    </a>
    <a class="button" href="https://chat.whatsapp.com/EQGWV7XklYy6MiBJ4JiQmt" target="_blank">
      <img src="https://i.imgur.com/jXweBHJ.png" alt="Divisa Hacking">
      GRUPO
    </a>
  </div>

  <div class="status fade-in">Online</div>
  <div class="quote fade-in">conhecido de onde eu vim e respeitado onde eu vou</div>

  <div class="info-boxes fade-in">
    <div class="info-box">
      <h2>SOBRE MIM</h2>
      <p>Conhecido como Árabe, sou o criador e administrador tanto da Divine quanto da Divisa Hacking. Comprometido em compartilhar conhecimento, métodos e conexões valiosas nesse universo digital juntamente com meu parceiro anguish.</p>
    </div>
    <div class="info-box">
      <h2>𝐃𝐈𝐕𝐈𝐍𝐄</h2>
      <p>A Divine é voltada para o vazamento de métodos, bots, logins e outros conteúdos exclusivos. Um canal direto para quem busca estratégias e ferramentas diferenciadas.</p>
    </div>
    <div class="info-box">
      <h2>DIVISA HACKING</h2>
      <p>O grupo Divisa Hacking serve para compartilhamento de conteúdo, interação entre membros e troca de informações relevantes. Um espaço aberto para quem vive o underground.</p>
    </div>
  </div>

  <div id="fullscreen" onclick="hideFullscreen()">
    <img src="https://i.imgur.com/qv2zzf3.jpeg" alt="Fullscreen Profile">
  </div>
<div class="products fade-in">
  <!-- Produto 1 - Números de WhatsApp -->
  <div class="product">
    <img src="https://i.imgur.com/NZvWdWx.jpeg" alt="Whatsapp Números">
    <h3>Whatsapp Números</h3>
    <p>Compre números de WhatsApp de outros países para expandir seus contatos e atividades.</p>
    <a href="https://wa.me/5513981935658?text=Gostaria%20de%20comprar%20n%C3%BAmeros%20de%20WhatsApp" target="_blank">Comprar Agora</a>
  </div>

  <!-- Produto 2 - Métodos do 7 -->
  <div class="product">
    <img src="https://i.imgur.com/rkdmfqv.jpeg" alt="Métodos do 7">
    <h3>Métodos do 7</h3>
    <p>Adquira métodos exclusivos para realizar operações no estilo 7 e maximizar seus ganhos.</p>
    <a href="https://wa.me/5513981935658?text=Gostaria%20de%20adquirir%20m%C3%A9todos%20do%207" target="_blank">Comprar Agora</a>
  </div>

  <!-- Produto 3 - Painéis de Investigações -->
  <div class="product">
    <img src="https://i.imgur.com/To6TDf5.jpeg" alt="Painéis de Investigações">
    <h3>Painéis de Investigações</h3>
    <p>Tenha acesso a painéis especializados para investigações e coleta de informações.</p>
    <a href="https://wa.me/5513981935658?text=Gostaria%20de%20adquirir%20pain%C3%A9is%20de%20investiga%C3%A7%C3%A3o" target="_blank">Comprar Agora</a>
  </div>

  <!-- Produto 4 - Banners Bolha -->
  <div class="product">
    <img src="https://i.imgur.com/CPMxKRB.jpeg" alt="Banners Bolha">
    <h3>Banners Bolha</h3>
    <p>Adquira banners bolha personalizados para promover suas atividades de forma impactante.</p>
    <a href="https://wa.me/5513981935658?text=Gostaria%20de%20adquirir%20banners%20bolha" target="_blank">Comprar Agora</a>
  </div>
</div>
  
  <script>
    function copyPhone() {
      navigator.clipboard.writeText("ㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤ🇸🇦ㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤ").then(() => {
        alert("Texto copiado!");
      });
    }

    function showFullscreen() {
      document.getElementById("fullscreen").style.display = "flex";
    }

    function hideFullscreen() {
      document.getElementById("fullscreen").style.display = "none";
    }

    window.addEventListener('load', () => {
      setTimeout(() => {
        document.querySelectorAll('.fade-in').forEach(el => el.classList.add('visible'));
      }, 2000);
    });

    window.addEventListener('scroll', () => {
      document.querySelectorAll('.fade-in').forEach(el => {
        const top = el.getBoundingClientRect().top;
        if (top < window.innerHeight - 100) {
          el.classList.add('visible');
        }
      });
    });
  </script>
</body>
</html>
