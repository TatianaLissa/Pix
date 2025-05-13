<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ambiente Virtual de Comunicação Pix</title>
    <style>
        body {
            background-color: pink;
            font-family: 'Times New Roman', serif;
        }
        h1 {
            text-align: center;
            font-family: Arial, sans-serif;
            color: black;
        }
        .texto {
            color: black;
            text-align: center;
        }
    </style>
</head>
<body>
    <h1>Ambiente Virtual de Comunicação Pix</h1>
    <p class="texto">O Pix foi lançado após o Plano Real e sua tradução para a língua inglesa é Real Time Payment ou RTP. O Pix permite pagamentos instantâneos quase em tempo real. Um dos objetivos foi diminuir a circulação de dinheiro em espécie. </p>
    <p class="texto">O Pix pode ser considerado seguro e as restrições feitas no geral a senhas muito fáceis de serem tidas incluem os acessos por mobile. </p>
    <p class="texto">O Pix é gratuito para pessoas físicas, tornou o processo de pagamentos mais rápido e acessível. </p>
</body>
</html>
   

<html>
<head>
    <title>Imagens</title>

<style>
        .image-container {
            margin-bottom: 20px; /* Adiciona um espaço entre as imagens */
        }
        .image-container img {
            width: 500px; /* Define uma largura padrão para as imagens */
            height: auto; /* Mantém a proporção das imagens */
            display: block; /* Garante que as imagens fiquem em blocos separados */
        }
    </style>
</head>
<body>

    <div class="image-container">
        <a href="https://photos.app.goo.gl/Sb7bZY3XcbkHsauAA" target="_blank">
            <img src="https://via.placeholder.com/500x300?text=Imagem+1" alt="Imagem 1">
        </a>
    </div>


 <div class="image-container">
        <a href="https://photos.app.goo.gl/8r9DMgmfZuZz721Y9" target="_blank">
            <img src="https://via.placeholder.com/500x300?text=Imagem+2" alt="Imagem 2">
        </a>
    </div>

    <div class="image-container">
        <a href="https://photos.app.goo.gl/nknGM8JgD4HUx8q59" target="_blank">
            <img src="https://via.placeholder.com/500x300?text=Imagem+3" alt="Imagem 3">
        </a>
    </div>

    <div class="image-container">
        <a href="https://photos.app.goo.gl/KU3N46ZGJJd13FcF8" target="_blank">
            <img src="https://via.placeholder.com/500x300?text=Imagem+4" alt="Imagem 4">
        </a>
    </div>

    <div class="image-container">
        <a href="https://photos.app.goo.gl/2N8cQuWsz5EkhAVk9" target="_blank">
            <img src="https://via.placeholder.com/500x300?text=Imagem+5" alt="Imagem 5">
        </a>
    </div>

    <div class="image-container">
        <a href="https://photos.app.goo.gl/KDxznukziJKqexqu7" target="_blank">
            <img src="https://via.placeholder.com/500x300?text=Imagem+6" alt="Imagem 6">
        </a>
    </div>

    <!DOCTYPE html>
<html lang="pt-br">
<head>
<meta charset="UTF-8" />
<title>Menu Horizontal com Formulário e Banco de Dados</title>
<style>
  body { font-family: Arial, sans-serif; margin: 0; }
  nav { background: #eee; border-bottom: 1px solid #ccc; }
  nav ul { list-style: none; margin: 0; padding: 0; display: flex; }
  nav ul li { flex: 1; text-align: center; }
  nav ul li a {
    display: block; padding: 10px 0; text-decoration: none; color: #333;
    border-right: 1px solid #ccc;
  }
  nav ul li:last-child a { border-right: none; }
  nav ul li a:hover { background: #ddd; }
  .content { padding: 20px; }
  form input, form textarea {
    display: block; margin-bottom: 10px; width: 100%; max-width: 400px; padding: 8px;
  }
  form button { padding: 8px 16px; }
  table { border-collapse: collapse; width: 100%; max-width: 600px; }
  table, th, td { border: 1px solid #ccc; }
  th, td { padding: 8px; text-align: left; }
</style>
</head>
<body>

<nav>
  <ul>
    <li><a href="#" onclick="showPage('1')">1</a></li>
    <li><a href="#" onclick="showPage('2')">2</a></li>
    <li><a href="#" onclick="showPage('3')">3</a></li>
    <li><a href="#" onclick="showPage('4')">Comunicação com as autoridades</a></li>
    <li><a href="#" onclick="showPage('5')">5</a></li>
  </ul>
</nav>

<div class="content" id="content">
  <!-- Conteúdo dinâmico será inserido aqui -->
</div>

<script>
  function showPage(page) {
    const content = document.getElementById('content');
    if (page === '1' || page === '2' || page === '3') {
      content.innerHTML = `<h2>Página ${page}</h2><p>Conteúdo da página ${page}.</p>`;
    } else if (page === '4') {
      content.innerHTML = `
        <h2>Comunicação com as autoridades</h2>
        <form id="contactForm">
          <input type="text" name="nome" placeholder="Nome" required />
          <input type="email" name="email" placeholder="Email" required />
          <textarea name="mensagem" placeholder="Mensagem" rows="5" required></textarea>
          <button type="submit">Enviar</button>
        </form>
        <p id="formStatus"></p>
      `;
      document.getElementById('contactForm').onsubmit = function(e) {
        e.preventDefault();
        const nome = this.nome.value.trim();
        const email = this.email.value.trim();
        const mensagem = this.mensagem.value.trim();
        if (nome && email && mensagem) {
          let dados = JSON.parse(localStorage.getItem('envios') || '[]');
          dados.push({ nome, email, mensagem, data: new Date().toLocaleString() });
          localStorage.setItem('envios', JSON.stringify(dados));
          this.reset();
          document.getElementById('formStatus').textContent = 'Enviado com sucesso!';
        }
      };
    } else if (page === '5') {
      let dados = JSON.parse(localStorage.getItem('envios') || '[]');
      if (dados.length === 0) {
        content.innerHTML = '<h2>Banco de Dados dos envios</h2><p>Nenhum envio registrado.</p>';
      } else {
        let tabela = `<h2>Banco de Dados dos envios</h2><table>
          <tr><th>Nome</th><th>Email</th><th>Mensagem</th><th>Data</th></tr>`;
        dados.forEach(d => {
          tabela += `<tr>
            <td>${d.nome}</td>
            <td>${d.email}</td>
            <td>${d.mensagem}</td>
            <td>${d.data}</td>
          </tr>`;
        });
        tabela += '</table>';
        content.innerHTML = tabela;
      }
    }
  }

  // Exibe a página 1 por padrão
  showPage('1');
</script>

</body>
</html>

