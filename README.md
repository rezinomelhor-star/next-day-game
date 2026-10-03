# next-day-game# Criando o arquivo index.html em um formato simples para garantir a geração do arquivo para download
html_content = """<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Meu Arquivo HTML</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f9;
            color: #333;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }
        .container {
            background: white;
            padding: 30px;
            border-radius: 12px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.1);
            text-align: center;
            max-width: 400px;
        }
        h1 {
            color: #2c3e50;
            font-size: 24px;
        }
        p {
            font-size: 16px;
            color: #666;
        }
        button {
            background-color: #3498db;
            color: white;
            border: none;
            padding: 10px 20px;
            font-size: 16px;
            border-radius: 6px;
            cursor: pointer;
            transition: background 0.3s;
            margin-top: 15px;
        }
        button:hover {
            background-color: #2980b9;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Página HTML Criada!</h1>
        <p>Este é um arquivo HTML completo com estrutura, estilos CSS e um toque de JavaScript.</p>
        <button onclick="mensagem()">Clique aqui</button>
    </div>

    <script>
        function mensagem() {
            alert('O seu arquivo HTML está funcionando perfeitamente!');
        }
    </script>
</body>
</html>
"""

filename = "index.html"
with open(filename, "w", encoding="utf-8") as f:
    f.write(html_content)

print(f"Arquivo {filename} criado com sucesso.")

