# plataforma-matematicas
from pathlib import Path
# Creamos un archivo HTML simple con estructura básica para una plataforma educativa
html_code = """
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Plataforma Matemáticas - Colegio América de Puebla</title>
  <style>
    body { font-family: Arial, sans-serif; margin: 0; padding: 0; background: #f4f4f4; }
    header { background: #003366; color: white; padding: 1em; text-align: center; }
    section { padding: 2em; }
    h2 { color: #003366; }
    .video-container { margin-bottom: 2em; }
    iframe { width: 100%; max-width: 560px; height: 315px; border: none; }
    footer { background: #003366; color: white; text-align: center; padding: 1em; margin-top: 2em; }
  </style>
</head>
<body>
  <header>
    <h1>Plataforma de Matemáticas</h1>
    <p>Apoyo educativo para estudiantes del Colegio América de Puebla</p>
  </header>

  <section>
    <h2>Álgebra</h2>
    <div class="video-container">
      <iframe src="https://www.youtube.com/embed/4gS6eQWo7b8" allowfullscreen></iframe>
    </div>
    <h2>Factorización</h2>
    <div class="video-container">
      <iframe src="https://www.youtube.com/embed/5VLqX2kkfn4" allowfullscreen></iframe>
    </div>
    <h2>Trigonometría</h2>
    <div class="video-container">
      <iframe src="https://www.youtube.com/embed/vqv3DpTfiTI" allowfullscreen></iframe>
    </div>
  </section>

  <footer>
    <p>© 2025 Plataforma Matemáticas | Colegio América de Puebla</p>
  </footer>
</body>
</html>
"""

# Guardamos el archivo HTML como index.html
output_dir = Path("/mnt/data")
output_path = output_dir / "index.html"
output_path.write_text(html_code, encoding="utf-8")

output_path.name
