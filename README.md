# basson
Development
from flask import Flask, render_template

app = Flask(__name__)

# Rota para a página inicial
@app.route("/")
def homepage():
    return render_template("homepage.html")

# Rota para a página de contatos
@app.route("/contatos")
def contatos():
    return render_template("contatos.html")

# Rota para uma página personalizada
@app.route("/usuarios/<nome_usuario>")
def usuarios(nome_usuario):
    return render_template("usuarios.html", nome_usuario=nome_usuario)

# Executar o servidor
if __name__ == "__main__":
    app.run(debug=True)
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Página com Fundo Branco</title>
    <style>
        body {
            background-color: #FFFFFF; /* Cor do fundo: Branco */
            font-family: Arial, sans-serif; /* Fonte padrão */
        }
    </style>
</head>
<body>
    <h1>Bem-vindo à minha página!</h1>
    <p>Esta página tem um fundo branco.</p>
</body>
</html>
