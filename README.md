# galinha
<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Loja de Galinhas do Zé</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #f9f9f9;
      color: #333;
      margin: 0;
      padding: 0;
    }
    header {
      background-color: #ffcc00;
      padding: 15px;
      text-align: center;
    }
    h1 {
      margin: 0;
    }
    .produtos {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 20px;
      padding: 20px;
    }
    .produto {
      background-color: white;
      border: 1px solid #ddd;
      border-radius: 10px;
      width: 250px;
      box-shadow: 2px 2px 8px rgba(0,0,0,0.1);
      text-align: center;
      padding: 10px;
    }
    .produto img {
      width: 100%;
      border-radius: 10px;
    }
    .btn {
      background-color: #ff6600;
      color: white;
      border: none;
      padding: 10px 15px;
      border-radius: 5px;
      cursor: pointer;
    }
    .btn:hover {
      background-color: #e55d00;
    }
    footer {
      text-align: center;
      padding: 10px;
      background-color: #ffcc00;
      position: fixed;
      bottom: 0;
      width: 100%;
    }
  </style>
</head>
<body>
  <header>
    <h1>🐔 Loja de Galinhas do Zé</h1>
    <p>As melhores galinhas caipiras da região!</p>
  </header>

  <section class="produtos">
    <div class="produto">
      <img src="https://images.unsplash.com/photo-1568640347023-d7b4b4e2c0f3" alt="Galinha Caipira">
      <h2>Galinha Caipira</h2>
      <p>R$ 50,00</p>
      <button class="btn" onclick="adicionarAoCarrinho('Galinha Caipira', 50)">Adicionar ao carrinho</button>
    </div>
    <div class="produto">
      <img src="https://images.unsplash.com/photo-1606813909358-5e6a7e1a3a3d" alt="Galo de Briga">
      <h2>Galo de Briga</h2>
      <p>R$ 120,00</p>
      <button class="btn" onclick="adicionarAoCarrinho('Galo de Briga', 120)">Adicionar ao carrinho</button>
    </div>
    <div class="produto">
      <img src="https://images.unsplash.com/photo-1617196035839-9b19e9c83c36" alt="Pintinho">
      <h2>Pintinho</h2>
      <p>R$ 10,00</p>
      <button class="btn" onclick="adicionarAoCarrinho('Pintinho', 10)">Adicionar ao carrinho</button>
    </div>
  </section>

  <footer>
    <p>&copy; 2025 Loja de Galinhas do Zé 🐣</p>
  </footer>

  <script>
    let carrinho = [];

    function adicionarAoCarrinho(produto, preco) {
      carrinho.push({ produto, preco });
      alert(`${produto} foi adicionado ao carrinho!`);
      console.log(carrinho);
    }
  </script>
</body>
</html>