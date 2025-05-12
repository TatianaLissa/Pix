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
    
</body>
</head>
   



        

<!DOCTYPE html>
<html lang="pt-br">
<head>
<meta charset="UTF-8" />
<title>Exemplo de Abas</title>
<style>
  /* Estilo das abas */
  .abas {
    list-style: none;
    padding: 0;
    margin: 0;
    display: flex;
    border-bottom: 1px solid #ccc;
  }
  .aba {
    margin-right: 5px;
  }
  .aba > a {
    display: block;
    padding: 10px 20px;
    background: #eee;
    color: #333;
    text-decoration: none;
    border: 1px solid #ccc;
    border-bottom: none;
    border-radius: 5px 5px 0 0;
  }
  .aba:not(:target) > a {
    background: #eee;
  }
  .aba:target > a, .aba > a:hover {
    background: white;
    font-weight: bold;
  }
  /* Conteúdo das abas */
  .conteudo {
    border: 1px solid #ccc;
    padding: 20px;
    background: white;
    display: none;
  }
  /* Exibe o conteúdo da aba selecionada */
  .aba:target .conteudo {
    display: block;
  }
  /* Exibe a primeira aba por padrão */
  .aba:first-child:target ~ .aba:first-child .conteudo,
  body:not(:target) .aba:first-child .conteudo {
    display: block;
  }
</style>
</head>
<body>

<ul class="abas">
  <li class="aba" id="aba1">
    <a href="#aba1">De onde vem o Pix?</a>
    <div class="conteudo">
     O Pix, o sistema de pagamentos instantâneos do Banco Central do Brasil, surgiu de estudos iniciados em 2016 com o objetivo de modernizar as transações financeiras, tornando-as mais rápidas, seguras e acessíveis. A ideia foi implementada e o Pix lançado em novembro de 2020, revolucionando a forma como os brasileiros realizam pagamentos e transferências. 
História e desenvolvimento:

    2016: Início dos estudos e planejamento para criação de um sistema de pagamentos instantâneos. 

2018: O Banco Central formaliza a iniciativa e um grupo de estudos é formado. 
2019-2020: Desenvolvimento do sistema, criação da marca e lançamento da campanha de divulgação. 
2020: Lançamento oficial do Pix para todos os usuários. 

Principais características:

    Rápido: As transações Pix são realizadas em poucos segundos. 

Seguro: O sistema utiliza tecnologia robusta para garantir a segurança das transações. 
Acessível: O Pix permite que qualquer pessoa, com acesso a um celular ou computador, faça pagamentos e transferências. 
Instantâneo: A liquidação das transações ocorre em poucos segundos. 
Gratuito: Em geral, as transações Pix não são cobradas pelas instituições financeiras. 

Impacto:

    Modernização:
    O Pix mudou a forma como os brasileiros realizam transações financeiras, substituindo métodos mais antigos e complexos. 

Inclusão financeira:
O Pix democratizou o acesso a pagamentos e transferências, permitindo que mais pessoas, especialmente aquelas que não tinham acesso a contas bancárias tradicionais, pudessem fazer transações. 
Novas possibilidades:
O Pix abre espaço para a criação de novas aplicações e serviços financeiros, impulsionando a inovação no setor. 
Transformação do varejo:
O Pix impactou a forma como as empresas vendem e como os consumidores compram, com a facilidade do pagamento à vista incentivando o uso da ferramenta. 


        
      

    </div>
  </li>
  <li class="aba" id="aba2">
    <a href="#aba2">Como e por quê usar o pix</a>
    <div class="conteudo">
     O PIX é um sistema de pagamentos instantâneos criado pelo Banco Central do Brasil que permite transferir dinheiro, pagar contas e receber pagamentos de forma rápida e fácil, a qualquer hora do dia, até mesmo em fins de semana e feriados. Para usar o PIX, você precisa cadastrar uma chave PIX no seu aplicativo bancário, que pode ser seu CPF, e-mail, número de telefone ou uma chave aleatória. 
Como usar o PIX:

    1. Cadastre uma chave PIX:
    No aplicativo do seu banco, siga as instruções para cadastrar uma chave PIX. 

2. Para pagar:

    Ler QR Code: Apunte a câmera do seu celular para o QR Code do recebedor. 

Informar a chave PIX: Digite ou selecione a chave PIX do recebedor. 

3. Para receber:

    Gerar QR Code: Gere um QR Code no seu aplicativo bancário e compartilhe com o pagador. 

Informar a chave PIX: Dê a sua chave PIX para o pagador. 

4. Confirme e finalize:
Confirme os dados e finalize a transação. 

Por que usar o PIX:

    Rapidez e praticidade: Os pagamentos e transferências são feitos em segundos, a qualquer momento. 

Segurança: O sistema é seguro e utiliza criptografia. 
Gratuidade: As transações entre pessoas físicas são gratuitas. 
Facilidade: Não precisa de boletos, agências bancárias ou esperar por compensações. 
Versatilidade: Pode ser usado em compras presenciais e online, para pagar contas e transferir dinheiro. 

        
      

    </div>
  </li>
  <li class="aba" id="aba4">
    <a href="#aba4">Fui lesado</a>
    <div class="conteudo">
     <!DOCTYPE html>
<html lang="pt-br">
<head>
<meta charset="UTF-8" />
<title>Campo de Denúncia</title>
</head>
<body>

<h2>Meus Dados</h2>

<form action="processa_denuncia.php" method="post">
  <label for="nome">Nome:</label><br />
  <input type="text" id="nome" name="nome" required><br /><br />

  <label for="email">E-mail:</label><br />
  <input type="email" id="email" name="email" required><br /><br />

  <label for="descricao">Descrição da denúncia:</label><br />
  <textarea id="descricao" name="descricao" rows="5" cols="40" required></textarea><br /><br />

  <button type="submit">Enviar denúncia</button>
</form>

</body>
</html>



      
    </div>
  </li>
  <li class="aba" id="aba5">
      a href="#aba5">Relatórios</a>" 
      <div class="conteúdo">
         <div class="tabs">
  <div class="tab active" data-tab="meuRelato">Meu relato</div>
  <div class="tab" data-tab="relatos">Relatos</div>
</div>

<div id="meuRelato" 
          
          
          class="tab-content" style="display:none;">
  <h2>Relatos enviados</h2>
  <ul id="relatosList">
    <!-- Relatos aparecerão aqui -->
  </ul>
</div>

<script>
  // Controle das abas
  const tabs = document.querySelectorAll('.tab');
  const contents = {
    meuRelato: document.getElementById('meuRelato'),
    relatos: document.getElementById('relatos')
  };

  tabs.forEach(tab => {
    tab.addEventListener('click', () => {
      tabs.forEach(t => t.classList.remove('active'));
      tab.classList.add('active');
      for (const key in contents) {
        contents[key].style.display = 'none';
      }
      contents[tab.dataset.tab].style.display = 'block';
      if(tab.dataset.tab === 'relatos') {
        carregarRelatos();
      }
    });
  });

  // Simula armazenamento local dos relatos
  function carregarRelatos() {
    const relatosList = document.getElementById('relatosList');
    relatosList.innerHTML = '';
    const relatos = JSON.parse(localStorage.getItem('relatos')) || [];
    if (relatos.length === 0) {
      relatosList.innerHTML = '<li>Nenhum relato enviado.</li>';
      return;
    }
    relatos.forEach((relato, i) => {
      const li = document.createElement('li');
      li.textContent = `${relato.nome}: ${relato.descricao}`;
      relatosList.appendChild(li);
    });
  }

  // Envio do formulário
  document.getElementById('formRelato').addEventListener('submit', function(e) {
    e.preventDefault();
    const nome = this.nome.value.trim();
    const descricao = this.descricao.value.trim();
    if(nome && descricao) {
      const relatos = JSON.parse(localStorage.getItem('relatos')) || [];
      relatos.push({ nome, descricao });
      localStorage.setItem('relatos', JSON.stringify(relatos));
      alert('Relato enviado com sucesso!');
      this.reset();
      // Muda para a aba Relatos para mostrar o novo relato
      tabs.forEach(t => t.classList.remove('active'));
      tabs[1].classList.add('active');
      contents.meuRelato.style.display = 'none';
      contents.relatos.style.display = 'block';
      carregarRelatos();
    }
  });
</script>
</body>
</html>



      
    </div>
  </li>
</ul>

</body>
</html>








            

