<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <title>Rose Mimo - Beleza, Mimos e Variedades</title>

  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600;700&display=swap" rel="stylesheet">

  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body {
      font-family: 'Poppins', sans-serif;
      background: #fff8fb;
      color: #333;
    }

    header {
      background: linear-gradient(135deg, #c2185b, #ff4fa3);
      color: white;
      text-align: center;
      padding: 22px 12px;
      box-shadow: 0 3px 10px rgba(0,0,0,0.15);
    }

    header h1 {
      font-size: 28px;
      font-weight: 700;
    }

    header p {
      margin-top: 6px;
      font-size: 14px;
    }

    .contato {
      margin-top: 8px;
      font-size: 13px;
    }

    main {
      padding: 18px 12px 100px;
      max-width: 1100px;
      margin: auto;
    }

    h2 {
      color: #c2185b;
      font-size: 21px;
      margin: 22px 0 12px;
      border-left: 5px solid #ff4fa3;
      padding-left: 10px;
    }

    .products {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      gap: 12px;
    }

    .card {
      background: white;
      border-radius: 14px;
      padding: 10px;
      box-shadow: 0 3px 10px rgba(0,0,0,0.10);
      text-align: center;
      overflow: hidden;
    }

    .card img {
      width: 100%;
      height: 145px;
      object-fit: cover;
      border-radius: 10px;
      background: #f8f8f8;
    }

    .card h3 {
      font-size: 14px;
      color: #c2185b;
      margin: 9px 0 5px;
      line-height: 1.3;
    }

    .card p {
      font-size: 11px;
      color: #666;
      min-height: 30px;
      line-height: 1.35;
    }

    .price {
      display: block;
      color: #111;
      font-size: 17px;
      font-weight: 700;
      margin: 8px 0;
    }

    .btn {
      width: 100%;
      border: none;
      border-radius: 20px;
      background: #c2185b;
      color: white;
      padding: 9px 5px;
      font-family: 'Poppins', sans-serif;
      font-weight: 600;
      font-size: 12px;
      cursor: pointer;
    }

    .btn:active {
      transform: scale(0.97);
    }

    /* CARRINHO */

    .cart-icon {
      position: fixed;
      right: 18px;
      bottom: 18px;
      width: 58px;
      height: 58px;
      border-radius: 50%;
      background: #c2185b;
      color: white;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 25px;
      box-shadow: 0 4px 15px rgba(0,0,0,0.25);
      z-index: 1000;
      cursor: pointer;
    }

    .cart-count {
      position: absolute;
      top: -4px;
      right: -2px;
      background: #ff4fa3;
      color: white;
      width: 22px;
      height: 22px;
      border-radius: 50%;
      font-size: 12px;
      font-weight: bold;
      display: flex;
      align-items: center;
      justify-content: center;
    }

    .cart {
      position: fixed;
      right: 10px;
      bottom: 85px;
      width: calc(100% - 20px);
      max-width: 420px;
      background: white;
      border-radius: 18px;
      box-shadow: 0 5px 25px rgba(0,0,0,0.25);
      padding: 18px;
      z-index: 999;
      display: none;
    }

    .cart.active {
      display: block;
    }

    .cart h3 {
      color: #c2185b;
      margin-bottom: 12px;
    }

    #itensCarrinho {
      max-height: 280px;
      overflow-y: auto;
    }

    .item-carrinho {
      display: flex;
      justify-content: space-between;
      align-items: center;
      gap: 8px;
      padding: 8px 0;
      border-bottom: 1px solid #eee;
      font-size: 12px;
    }

    .item-carrinho button {
      border: none;
      background: #ff4fa3;
      color: white;
      border-radius: 50%;
      width: 24px;
      height: 24px;
      cursor: pointer;
    }

    .total {
      font-size: 18px;
      font-weight: 700;
      margin: 14px 0;
      color: #c2185b;
    }

    .finalizar {
      width: 100%;
      padding: 12px;
      border: none;
      border-radius: 25px;
      background: #25D366;
      color: white;
      font-size: 15px;
      font-weight: 700;
      font-family: 'Poppins', sans-serif;
      cursor: pointer;
    }

    .fechar {
      width: 100%;
      margin-top: 8px;
      padding: 9px;
      border: none;
      border-radius: 20px;
      background: #eee;
      color: #555;
      font-family: 'Poppins', sans-serif;
      cursor: pointer;
    }

    footer {
      text-align: center;
      padding: 25px 10px;
      background: #c2185b;
      color: white;
      font-size: 12px;
    }

    @media (min-width: 600px) {
      .products {
        grid-template-columns: repeat(3, 1fr);
      }
    }

    @media (min-width: 900px) {
      .products {
        grid-template-columns: repeat(4, 1fr);
      }
    }
  </style>
</head>

<body>

<header>
  <h1>👑 ROSE MIMO 🌹</h1>
  <p>Beleza, Mimos e Variedades</p>
  <div class="contato">
    WhatsApp: (85) 98700-5202 | @mimosdarosevariedades
  </div>
</header>

<main>

  <!-- =========================
       MAQUIAGEM
  ========================== -->

  <h2>💄 Maquiagem</h2>

  <div class="products">

    <div class="card">
      <img src="https://uploads.onecompiler.io/454bxpyrs/1790380427349/Blush-duo.jpg" alt="Blush Compacto Duo Ruby Rose">
      <h3>Blush Compacto Duo Ruby Rose</h3>
      <p>Blush compacto duo</p>
      <span class="price">R$ 10,00</span>
      <button class="btn" onclick="add('Blush Compacto Duo Ruby Rose',10)">Adicionar</button>
    </div>

    <div class="card">
      <img src="https://uploads.onecompiler.io/454bxpyrs/1790380377046/Blush%20compactado.jpg" alt="Blush Compacto Playback">
      <h3>Blush Compacto Playback</h3>
      <p>Blush compacto</p>
      <span class="price">R$ 14,00</span>
      <button class="btn" onclick="add('Blush Compacto Playback',14)">Adicionar</button>
    </div>

    <div class="card">
      <img src="https://uploads.onecompiler.io/454bxpyrs/1790380737219/delineador.jpg" alt="Delineador Ultra Black Vivai">
      <h3>Delineador Ultra Black Vivai</h3>
      <p>Delineador preto intenso</p>
      <span class="price">R$ 12,00</span>
      <button class="btn" onclick="add('Delineador Ultra Black Vivai',12)">Adicionar</button>
    </div>

    <div class="card">
      <img src="https://uploads.onecompiler.io/454bxpyrs/1790380853563/Lapis-pink21.jpg" alt="Lápis Olho e Lábio Pink21">
      <h3>Lápis Olho e Lábio Pink21</h3>
      <p>Lápis para olhos e lábios</p>
      <span class="price">R$ 5,00</span>
      <button class="btn" onclick="add('Lápis Olho e Lábio Pink21',5)">Adicionar</button>
    </div>

    <div class="card">
      <img src="https://uploads.onecompiler.io/454bxpyrs/1790380873943/P%C3%83%C2%B3%20compacto.jpg" alt="Pó Compacto Popstar">
      <h3>Pó Compacto Popstar</h3>
      <p>Pó compacto para maquiagem</p>
      <span class="price">R$ 10,00</span>
      <button class="btn" onclick="add('Pó Compacto Popstar',10)">Adicionar</button>
    </div>

    <div class="card">
      <img src="https://uploads.onecompiler.io/454bxpyrs/1790380888554/P%C3%83%C2%B3%20de%20banana.jpg" alt="Pó de Banana Swiss Beauty">
      <h3>Pó de Banana Swiss Beauty</h3>
      <p>Pó facial</p>
      <span class="price">R$ 10,00</span>
      <button class="btn" onclick="add('Pó de Banana Swiss Beauty',10)">Adicionar</button>
    </div>

    <div class="card">
      <img src="https://uploads.onecompiler.io/454bxpyrs/1790380724811/esponja.jpg" alt="Esponja Chanfrada">
      <h3>Esponja Chanfrada</h3>
      <p>Esponja para maquiagem</p>
      <span class="price">R$ 5,00</span>
      <button class="btn" onclick="add('Esponja Chanfrada',5)">Adicionar</button>
    </div>

    <div class="card">
      <img src="https://uploads.onecompiler.io/454bxpyrs/1790381065318/Mascara-cilios.jpg" alt="Máscara de Cílios">
      <h3>Máscara de Cílios</h3>
      <p>Máscara para cílios</p>
      <span class="price">R$ 10,00</span>
      <button class="btn" onclick="add('Máscara de Cílios',10)">Adicionar</button>
    </div>

    <div class="card">
      <img src="https://uploads.onecompiler.io/454bxpyrs/1790380442611/brilho-labial.jpg" alt="Brilho Labial">
      <h3>Brilho Labial</h3>
      <p>Brilho para os lábios</p>
      <span class="price">R$ 10,00</span>
      <button class="btn" onclick="add('Brilho Labial',10)">Adicionar</button>
    </div>

    <div class="card">
      <img src="https://uploads.onecompiler.io/454bxpyrs/1791479720261/IMG-20261008-WA2271.jpg" alt="Batom da Vovó">
      <h3>Batom da Vovó</h3>
      <p>Batom</p>
      <span class="price">R$ 5,00</span>
      <button class="btn" onclick="add('Batom da Vovó',5)">Adicionar</button>
    </div>

    <div class="card">
      <img src="https://uploads.onecompiler.io/454bxpyrs/1791479785366/IMG-20261008-WA6053.jpg" alt="Gloss Variados">
      <h3>Gloss Variados</h3>
      <p>Escolha um gloss por apenas R$ 10,00</p>
      <span class="price">R$ 10,00</span>
      <button class="btn" onclick="add('Gloss Variados',10)">Adicionar</button>
    </div>

    <div class="card">
      <img src="https://uploads.onecompiler.io/454bxpyrs/1791479840305/IMG-20261008-WA2106.jpg" alt="Espelhinho com 5 Pincéis">
      <h3>Espelhinho com 5 Pincéis</h3>
      <p>Espelho com kit de pincéis</p>
      <span class="price">R$ 10,00</span>
      <button class="btn" onclick="add('Espelhinho com 5 Pincéis',10)">Adicionar</button>
    </div>

    <div class="card">
      <img src="https://uploads.onecompiler.io/454bxpyrs/1791479940186/IMG-20261008-WA9113.jpg" alt="Blindagem Facial">
      <h3>Blindagem Facial</h3>
      <p>Blindagem para preparação da pele</p>
      <span class="price">R$ 18,00</span>
      <button class="btn" onclick="add('Blindagem Facial',18)">Adicionar</button>
    </div>

    <div class="card">
      <img src="https://uploads.onecompiler.io/454bxpyrs/1791479850016/IMG-20261008-WA6366.jpg" alt="Lápis de Olho Popstar Ruby Rose">
      <h3>Lápis de Olho Popstar Ruby Rose</h3>
      <p>Lápis para olhos</p>
      <span class="price">R$ 6,00</span>
      <button class="btn" onclick="add('Lápis de Olho Popstar Ruby Rose',6)">Adicionar</button>
    </div>

    <div class="card">
      <img src="https://uploads.onecompiler.io/454bxpyrs/1791479860628/IMG-20261008-WA3355.jpg" alt="Corretivo Líquido">
      <h3>Corretivo Líquido</h3>
      <p>Escolha sua tonalidade pelo WhatsApp</p>
      <span class="price">R$ 12,00</span>
      <button class="btn" onclick="add('Corretivo Líquido',12)">Adicionar</button>
    </div>

  </div>


  <!-- =========================
       CUIDADOS COM A PELE
  ========================== -->

  <h2>🧖‍♀️ Cuidados com a Pele</h2>

  <div class="products">

    <div class="card">
      <img src="https://uploads.onecompiler.io/454bxpyrs/1790380245557/Agua-micelar.jpg" alt="Água Micelar">
      <h3>Água Micelar</h3>
      <p>Limpeza e cuidado facial</p>
      <span class="price">R$ 12,00</span>
      <button class="btn" onclick="add('Água Micelar',12)">Adicionar</button>
    </div>

    <div class="card">
      <img src="https://uploads.onecompiler.io/454bxpyrs/1791480038424/IMG-20261008-WA0807.jpg" alt="Hidratante Facial Bella Bem Me Quero">
      <h3>Hidratante Facial Bella Bem Me Quero 100 g</h3>
      <p>Hidratante facial</p>
      <span class="price">R$ 10,00</span>
      <button class="btn" onclick="add('Hidratante Facial Bella Bem Me Quero 100 g',10)">Adicionar</button>
    </div>

    <div class="card">
      <img src="https://uploads.onecompiler.io/454bxpyrs/1791480050598/IMG-20261008-WA5102.jpg" alt="Sabonete Líquido Bella Bem Me Quero">
      <h3>Sabonete Líquido Bella Bem Me Quero Make Up 100 ml</h3>
      <p>Sabonete líquido facial</p>
      <span class="price">R$ 10,00</span>
      <button class="btn" onclick="add('Sabonete Líquido Bella Bem Me Quero Make Up 100 ml',10)">Adicionar</button>
    </div>

    <div class="card">
      <img src="https://uploads.onecompiler.io/454bxpyrs/1791480017148/IMG-20261008-WA8030.jpg" alt="Sabonete Facial Rosa Mosqueta">
      <h3>Sabonete Facial Rosa Mosqueta Dermachem 100 ml</h3>
      <p>Sabonete facial</p>
      <span class="price">R$ 12,00</span>
      <button class="btn" onclick="add('Sabonete Facial Rosa Mosqueta Dermachem 100 ml',12)">Adicionar</button>
    </div>

    <div class="card">
      <img src="https://uploads.onecompiler.io/454bxpyrs/1791480006615/IMG-20261008-WA1758.jpg" alt="Faixa Lacinho">
      <h3>Faixa Lacinho</h3>
      <p>Faixa para cuidados faciais</p>
      <span class="price">R$ 10,00</span>
      <button class="btn" onclick="add('Faixa Lacinho',10)">Adicionar</button>
    </div>

  </div>


  <!-- =========================
       CUIDADOS E HIGIENE
  ========================== -->

  <h2>🧴 Cuidados e Higiene</h2>

  <div class="products">

    <div class="card">
      <img src="https://uploads.onecompiler.io/454bxpyrs/1790381126635/Sabonete-abacaxi.jpg" alt="Sabonete 1L">
      <h3>Sabonete 1L</h3>
      <p>Sabonete líquido</p>
      <span class="price">R$ 10,00</span>
      <button class="btn" onclick="add('Sabonete 1L',10)">Adicionar</button>
    </div>

    <div class="card">
      <img src="https://uploads.onecompiler.io/454bxpyrs/1790381317788/Escova%20de%20cabelo.jpg" alt="Escova de Cabelo">
      <h3>Escova de Cabelo</h3>
      <p>Escova para cabelos</p>
      <span class="price">R$ 10,00</span>
      <button class="btn" onclick="add('Escova de Cabelo',10)">Adicionar</button>
    </div>

    <div class="card">
      <img src="https://uploads.onecompiler.io/454bxpyrs/1790381330397/Escova%20massageadora.jpg" alt="Escova Massageadora">
      <h3>Escova Massageadora</h3>
      <p>Escova massageadora</p>
      <span class="price">R$ 8,00</span>
      <button class="btn" onclick="add('Escova Massageadora',8)">Adicionar</button>
    </div>

    <div class="card">
      <img src="https://uploads.onecompiler.io/454bxpyrs/1790381138795/d.jpg" alt="Esfoliante Rosto e Corpo">
      <h3>Esfoliante Rosto e Corpo</h3>
      <p>Esfoliante corporal e facial</p>
      <span class="price">R$ 20,00</span>
      <button class="btn" onclick="add('Esfoliante Rosto e Corpo',20)">Adicionar</button>
    </div>

    <div class="card">
      <img src="https://uploads.onecompiler.io/454bxpyrs/1790381157498/sintimo.jpg" alt="Sabonete Íntimo">
      <h3>Sabonete Íntimo</h3>
      <p>Higiene íntima</p>
      <span class="price">R$ 12,00</span>
      <button class="btn" onclick="add('Sabonete Íntimo',12)">Adicionar</button>
    </div>

    <div class="card">
      <img src="https://uploads.onecompiler.io/454bxpyrs/1790381253749/touca.jpg" alt="Touca de Cetim">
      <h3>Touca de Cetim</h3>
      <p>Proteção para os cabelos</p>
      <span class="price">R$ 5,00</span>
      <button class="btn" onclick="add('Touca de Cetim',5)">Adicionar</button>
    </div>

    <div class="card">
      <img src="https://uploads.onecompiler.io/454bxpyrs/1791480182549/IMG-20261008-WA8548.jpg" alt="Hidratante Desodorante Corporal Bio Instinto">
      <h3>Hidratante Desodorante Corporal Bio Instinto 400 ml</h3>
      <p>Hidratante corporal</p>
      <span class="price">R$ 20,00</span>
      <button class="btn" onclick="add('Hidratante Desodorante Corporal Bio Instinto 400 ml',20)">Adicionar</button>
    </div>

    <div class="card">
      <img src="https://uploads.onecompiler.io/454bxpyrs/1791480285849/IMG-20261008-WA5589.jpg" alt="Máscara Capilar Lolise">
      <h3>Máscara Capilar Lolise Nutrição Profunda 3 em 1 500 g</h3>
      <p>Nutrição profunda para os cabelos</p>
      <span class="price">R$ 20,00</span>
      <button class="btn" onclick="add('Máscara Capilar Lolise Nutrição Profunda 3 em 1 500 g',20)">Adicionar</button>
    </div>

    <div class="card">
      <img src="https://uploads.onecompiler.io/454bxpyrs/1791480192930/IMG-20261008-WA2941.jpg" alt="Body Splash Bio Instinto">
      <h3>Body Splash Bio Instinto 130 ml</h3>
      <p>Body splash perfumado</p>
      <span class="price">R$ 20,00</span>
      <button class="btn" onclick="add('Body Splash Bio Instinto 130 ml',20)">Adicionar</button>
    </div>

    <div class="card">
      <img src="https://uploads.onecompiler.io/454bxpyrs/1791480318965/IMG-20261008-WA9962.jpg" alt="Sérum Dermachem">
      <h3>Sérum Dermachem 30 ml</h3>
      <p>Sérum facial</p>
      <span class="price">R$ 13,90</span>
      <button class="btn" onclick="add('Sérum Dermachem 30 ml',13.90)">Adicionar</button>
    </div>

    <div class="card">
      <img src="https://uploads.onecompiler.io/454bxpyrs/1791480204722/IMG-20261008-WA6668.jpg" alt="Body Splash Belkit">
      <h3>Body Splash Belkit 200 ml</h3>
      <p>Body splash perfumado</p>
      <span class="price">R$ 30,00</span>
      <button class="btn" onclick="add('Body Splash Belkit 200 ml',30)">Adicionar</button>
    </div>

    <div class="card">
      <img src="https://uploads.onecompiler.io/454bxpyrs/1791479576098/IMG-20261008-WA0410.jpg" alt="Sensações Banho de Lua">
      <h3>Sensações Banho de Lua Elas Cosméticos</h3>
      <p>Kit com 5 itens</p>
      <span class="price">R$ 13,00</span>
      <button class="btn" onclick="add('Sensações Banho de Lua Elas Cosméticos - 5 itens',13)">Adicionar</button>
    </div>

    <div class="card">
      <img src="https://uploads.onecompiler.io/454bxpyrs/1791480298344/IMG-20261008-WA3738.jpg" alt="Reparador de Pontas Luff">
      <h3>Reparador de Pontas Luff 30 ml</h3>
      <p>Cuidados para os cabelos</p>
      <span class="price">R$ 9,90</span>
      <button class="btn" onclick="add('Reparador de Pontas Luff 30 ml',9.90)">Adicionar</button>
    </div>

    <div class="card">
      <img src="https://uploads.onecompiler.io/454bxpyrs/1791480310881/IMG-20261008-WA9915.jpg" alt="Óleo Rosa Mosqueta">
      <h3>Óleo Rosa Mosqueta Lolise 60 ml</h3>
      <p>Óleo para cuidados</p>
      <span class="price">R$ 11,99</span>
      <button class="btn" onclick="add('Óleo Rosa Mosqueta Lolise 60 ml',11.99)">Adicionar</button>
    </div>

  </div>


  <!-- =========================
       ACESSÓRIOS E VARIEDADES
  ========================== -->

  <h2>💖 Acessórios e Variedades</h2>

  <div class="products">

    <div class="card">
      <img src="https://uploads.onecompiler.io/454bxpyrs/1790381435300/Xuxinha.jpg" alt="Xuxinha Cetim">
      <h3>Xuxinha Cetim</h3>
      <p>Elástico de cetim</p>
      <span class="price">R$ 3,00</span>
      <button class="btn" onclick="add('Xuxinha Cetim',3)">Adicionar</button>
    </div>

    <div class="card">
      <img src="https://uploads.onecompiler.io/454bxpyrs/1790381832502/Len%C3%83%C2%A7o%20umedecido%20P.jpg" alt="Lenço Fácil P Yasmim">
      <h3>Lenço Fácil P Yasmim</h3>
      <p>Lenço umedecido</p>
      <span class="price">R$ 5,00</span>
      <button class="btn" onclick="add('Lenço Fácil P Yasmim',5)">Adicionar</button>
    </div>

    <div class="card">
      <img src="https://uploads.onecompiler.io/454bxpyrs/1790381738367/Len%C3%83%C2%A7o%20umedecido%20G.jpg" alt="Lenço Fácil G">
      <h3>Lenço Fácil G</h3>
      <p>Lenço umedecido</p>
      <span class="price">R$ 8,00</span>
      <button class="btn" onclick="add('Lenço Fácil G',8)">Adicionar</button>
    </div>

    <div class="card">
      <img src="https://uploads.onecompiler.io/454bxpyrs/1791480465150/IMG-20261008-WA6095.jpg" alt="Piranhas Diversas">
      <h3>Piranhas Diversas</h3>
      <p>Escolha sua piranha — de R$ 5,00 a R$ 12,00</p>
      <span class="price">R$ 5,00 a R$ 12,00</span>
      <button class="btn" onclick="add('Piranhas Diversas - confirmar modelo pelo WhatsApp',5)">Adicionar</button>
    </div>

    <div class="card">
      <img src="https://uploads.onecompiler.io/454bxpyrs/1791480457226/IMG-20261008-WA2001.jpg" alt="Cartela de Presilhas de Estrelinha">
      <h3>Cartela de Presilhas de Estrelinha</h3>
      <p>Cartela de presilhas</p>
      <span class="price">R$ 10,00</span>
      <button class="btn" onclick="add('Cartela de Presilhas de Estrelinha',10)">Adicionar</button>
    </div>

    <div class="card">
      <img src="https://uploads.onecompiler.io/454bxpyrs/1791480475306/IMG-20261008-WA7079.jpg" alt="Piranha Infantil">
      <h3>Piranha Infantil</h3>
      <p>Cartelinha com 2 unidades</p>
      <span class="price">R$ 5,00</span>
      <button class="btn" onclick="add('Piranha Infantil - Cartelinha com 2 unidades',5)">Adicionar</button>
    </div>

    <div class="card">
      <img src="https://uploads.onecompiler.io/454bxpyrs/1791480502401/IMG-20261008-WA3691.jpg" alt="Liguinhas Coloridas">
      <h3>Liguinhas Coloridas</h3>
      <p>Liguinhas coloridas para cabelo</p>
      <span class="price">R$ 4,00</span>
      <button class="btn" onclick="add('Liguinhas Coloridas',4)">Adicionar</button>
    </div>

  </div>

</main>


<!-- =========================
     CARRINHO
========================== -->

<div class="cart-icon" onclick="toggle()">
  🛒
  <span class="cart-count" id="contador">0</span>
</div>

<div class="cart" id="carrinhoBox">

  <h3>🛒 Carrinho</h3>

  <div id="itensCarrinho">
    <p>Seu carrinho está vazio.</p>
  </div>

  <div class="total">
    Total: R$ <span id="total">0,00</span>
  </div>

  <label for="pagamento" style="display:block; color:#c2185b; font-weight:600; font-size:13px; margin:8px 0 6px;">
    💳 Forma de pagamento
  </label>

  <select id="pagamento" style="width:100%; padding:11px; border:1px solid #ddd; border-radius:12px; background:#fff; color:#333; font-family:'Poppins',sans-serif; font-size:13px; margin-bottom:10px;">
    <option value="">Selecione uma forma de pagamento</option>
    <option value="Pix">Pix</option>
    <option value="Dinheiro">Dinheiro</option>
    <option value="Cartão de crédito">Cartão de crédito</option>
    <option value="Cartão de débito">Cartão de débito</option>
  </select>

  <button class="finalizar" onclick="zap()">
    💚 Finalizar pelo WhatsApp
  </button>

  <button class="fechar" onclick="toggle()">
    Fechar
  </button>

</div>


<footer>
  🌹 Rose Mimo — Beleza, Mimos e Variedades 🌹
  <br>
  Siga: @mimosdarosevariedades
</footer>


<script>

  let carrinho = [];

  function add(nome, preco) {
    carrinho.push({
      nome: nome,
      preco: preco
    });

    upd();
    document.getElementById("carrinhoBox").classList.add("active");
  }

  function remover(index) {
    carrinho.splice(index, 1);
    upd();
  }

  function upd() {

    const itens = document.getElementById("itensCarrinho");
    const total = document.getElementById("total");
    const contador = document.getElementById("contador");

    contador.textContent = carrinho.length;

    if (carrinho.length === 0) {
      itens.innerHTML = "<p>Seu carrinho está vazio.</p>";
      total.textContent = "0,00";
      return;
    }

    let soma = 0;

    itens.innerHTML = "";

    carrinho.forEach((item, index) => {

      soma += item.preco;

      itens.innerHTML += `
        <div class="item-carrinho">
          <span>
            ${item.nome}<br>
            R$ ${item.preco.toFixed(2).replace('.', ',')}
          </span>

          <button onclick="remover(${index})">
            ×
          </button>
        </div>
      `;

    });

    total.textContent = soma.toFixed(2).replace('.', ',');
  }

  function toggle() {

    const box = document.getElementById("carrinhoBox");

    box.classList.toggle("active");

  }

  function zap() {

    if (carrinho.length === 0) {
      alert("Seu carrinho está vazio!");
      return;
    }

    const pagamento = document.getElementById("pagamento").value;

    if (!pagamento) {
      alert("Escolha a forma de pagamento antes de finalizar a compra.");
      document.getElementById("pagamento").focus();
      return;
    }

    let mensagem = "Olá! Quero fazer um pedido na Rose Mimo 🌹%0A%0A";

    let total = 0;

    carrinho.forEach((item, index) => {

      mensagem += `${index + 1}. ${item.nome} - R$ ${item.preco.toFixed(2).replace('.', ',')}%0A`;

      total += item.preco;

    });

    mensagem += `%0ATotal: R$ ${total.toFixed(2).replace('.', ',')}`;
    mensagem += `%0AForma de pagamento: ${pagamento}`;

    const numero = "5585987005202";

    window.open(
      `https://wa.me/${numero}?text=${mensagem}`,
      "_blank"
    );

  }

</script>

</body>
</html>
