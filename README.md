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
