import os
import zipfile

# Estrutura de diretórios e arquivos
project_name = "meu-primeiro-projeto"
base_path = f"/mnt/data/{project_name}"

# Criar diretório principal
os.makedirs(base_path, exist_ok=True)

# Criar index.html
index_html = """<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <title>Meu Primeiro Projeto</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <h1>Olá, sou o Lucas Vinícius!</h1>
    <p>Este é meu primeiro projeto no GitHub 🚀</p>
</body>
</html>
"""
with open(f"{base_path}/index.html", "w", encoding="utf-8") as f:
    f.write(index_html)

# Criar style.css
style_css = """body {
    font-family: Arial, sans-serif;
    background-color: #f4f4f9;
    color: #333;
    text-align: center;
    padding: 50px;
}

h1 {
    color: #0056b3;
}
"""
with open(f"{base_path}/style.css", "w", encoding="utf-8") as f:
    f.write(style_css)

zip_path
