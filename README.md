# contemporary-art
<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Galeria de Arte Contemporânea</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>

  <header class="header">
    <h1>Arte Contemporânea</h1>
    <p>Explorando formas, conceitos e expressões da era moderna</p>
  </header>

  <main class="gallery-container">
    <article class="card">
      <img src="https://images.unsplash.com/photo-1579783902614-a3fb3927b675?auto=format&fit=crop&w=600&q=80" alt="Pintura Abstrata">
      <div class="card-content">
        <h3>Pintura Abstrata</h3>
        <p>Expressão de emoções e conceitos visuais através de formas não representacionais e paletas vibrantes.</p>
      </div>
    </article>

    <article class="card">
      <img src="https://images.unsplash.com/photo-1541701494587-cb58502866ab?auto=format&fit=crop&w=600&q=80" alt="Arte Digital e Luz">
      <div class="card-content">
        <h3>Instalações Luminosas</h3>
        <p>Uso de tecnologia, projeções e luzes LED para transformar a percepção do espaço arquitetônico.</p>
      </div>
    </article>

    <article class="card">
      <img src="https://images.unsplash.com/photo-1543857778-c4a1a3e0b2eb?auto=format&fit=crop&w=600&q=80" alt="Escultura Moderna">
      <div class="card-content">
        <h3>Escultura Tridimensional</h3>
        <p>Desafio aos materiais tradicionais utilizando metal, acrílico e materiais reciclados em novas formas.</p>
      </div>
    </article>
  </main>

  <footer class="footer">
    <p>&copy; 2026 Galeria Contemporânea. Hospedado via GitHub Pages.</p>
  </footer>

</body>
</html>

:root {
  --bg-color: #0f0f11;
  --card-bg: #1a1a1e;
  --text-primary: #f0f0f5;
  --text-secondary: #a0a0b0;
  --accent: #6c5ce7;
}

* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

body {
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Helvetica, Arial, sans-serif;
  background-color: var(--bg-color);
  color: var(--text-primary);
  line-height: 1.6;
  display: flex;
  flex-direction: column;
  min-height: 100vh;
}

.header {
  text-align: center;
  padding: 3rem 1rem 2rem;
}

.header h1 {
  font-size: 2.5rem;
  letter-spacing: -1px;
  margin-bottom: 0.5rem;
}

.header p {
  color: var(--text-secondary);
  font-size: 1.1rem;
}

.gallery-container {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 2rem;
  max-width: 1200px;
  margin: 0 auto;
  padding: 2rem;
  flex: 1;
}

.card {
  background-color: var(--card-bg);
  border-radius: 12px;
  overflow: hidden;
  box-shadow: 0 4px 20px rgba(0, 0, 0, 0.4);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.card:hover {
  transform: translateY(-8px);
  box-shadow: 0 12px 30px rgba(108, 92, 231, 0.2);
}

.card img {
  width: 100%;
  height: 250px;
  object-fit: cover;
  display: block;
}

.card-content {
  padding: 1.5rem;
}

.card-content h3 {
  font-size: 1.3rem;
  margin-bottom: 0.5rem;
}

.card-content p {
  color: var(--text-secondary);
  font-size: 0.95rem;
}

.footer {
  text-align: center;
  padding: 2rem;
  color: var(--text-secondary);
  font-size: 0.9rem;
  border-top: 1px solid #2a2a30;
}
