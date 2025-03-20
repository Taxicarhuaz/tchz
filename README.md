<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Servicio de Taxi</title>
    <style>
        body {
            font-family: 'Poppins', sans-serif;
            margin: 0;
            padding: 0;
            text-align: center;
            background-color: #f4f4f4;
        }
        header {
            background-color: #ffcc00;
            padding: 20px;
            font-size: 28px;
            font-weight: bold;
            color: #333;
            box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.2);
        }
        section {
            padding: 20px;
            background: white;
            margin: 30px auto;
            width: 90%;
            max-width: 500px;
            border-radius: 10px;
            box-shadow: 0px 4px 15px rgba(0, 0, 0, 0.2);
            transition: transform 0.3s ease-in-out;
        }
        section:hover {
            transform: scale(1.02);
        }
        .btn {
            display: inline-block;
            background-color: #ffcc00;
            padding: 12px 24px;
            text-decoration: none;
            color: black;
            font-weight: bold;
            border-radius: 8px;
            margin-top: 15px;
            border: none;
            cursor: pointer;
            transition: background 0.3s;
        }
        .btn:hover {
            background-color: #e6b800;
        }
        form {
            display: flex;
            flex-direction: column;
            align-items: center;
        }
        input {
            padding: 12px;
            margin: 8px;
            width: 90%;
            max-width: 400px;
            border: 2px solid #ddd;
            border-radius: 8px;
            font-size: 16px;
            transition: border-color 0.3s;
        }
        input:focus {
            border-color: #ffcc00;
            outline: none;
        }
        #chat-widget {
            position: fixed;
            bottom: 20px;
            right: 20px;
            background-color: #ffcc00;
            padding: 12px 20px;
            border-radius: 25px;
            cursor: pointer;
            box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.3);
            font-weight: bold;
            font-size: 14px;
        }
        #chat-widget:hover {
            background-color: #e6b800;
        }
    </style>
</head>
<body>
    <header>
        <h1>🚖 Servicio de Taxi 24/7 🚖</h1>
    </header>
    <section>
        <h2>Reserva tu Taxi</h2>
        <form action="https://formspree.io/f/tu_formulario" method="POST">
            <input type="text" name="nombre" placeholder="Tu Nombre" required>
            <input type="text" name="recogida" placeholder="Ubicación de Recogida" required>
            <input type="text" name="destino" placeholder="Ubicación de Destino" required>
            <input type="tel" name="telefono" placeholder="Tu Teléfono" required>
            <input type="date" name="fecha" required>
            <input type="time" name="hora" required>
            <button class="btn" type="submit">Reservar Ahora</button>
        </form>
    </section>
    <div id="chat-widget" onclick="openChat()">
        ¿Requieres ayuda?
    </div>
    <script>
        function openChat() {
            window.open('https://wa.me/921427835', '_blank');
        }
    </script>
</body>
</html>
