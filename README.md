<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>YoLo - Control del Robot</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <header>
        <h1>YoLo 🤖</h1>
        <p>Panel de control del robot</p>
    </header>

    <main>
        <section class="camera">
            <h2>Cámara del robot</h2>
            <img id="video" src="" alt="Cámara desconectada">
            <p id="cameraStatus">Cámara desconectada</p>
        </section>

        <section class="controls">
            <h2>Movimiento</h2>

            <div class="buttons">
                <button onclick="move('adelante')">⬆ Adelante</button>

                <div class="middle">
                    <button onclick="move('izquierda')">⬅ Izquierda</button>
                    <button onclick="move('detener')">⏹ Detener</button>
                    <button onclick="move('derecha')">➡ Derecha</button>
                </div>

                <button onclick="move('atras')">⬇ Atrás</button>
            </div>
        </section>

        <section class="status">
            <h2>Estado</h2>
            <p id="status">Esperando conexión...</p>
        </section>
    </main>

    <footer>
        <p>Proyecto YoLo - Software II y Redes I</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>
