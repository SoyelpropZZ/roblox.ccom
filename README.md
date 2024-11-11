<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Inicio de Sesión</title>
    <link rel="stylesheet" href="css/styles.css">
</head>
<body>
    <div class="login-container">
        <h1>Iniciar sesión</h1>
        <form id="loginForm">
            <input type="text" placeholder="Nombre de usuario" id="username" required>
            <input type="password" placeholder="Contraseña" id="password" required>
            <button type="submit">Iniciar sesión</button>
        </form>
    </div>
    <script src="js/script.js"></script>
</body>
</html>
// script.js
document.getElementById('loginForm').addEventListener('submit', function(event) {
    event.preventDefault(); // Evita el envío del formulario para la demostración
    const username = document.getElementById('username').value;
    const password = document.getElementById('password').value;
    alert(`Usuario: ${username}\nContraseña: ${password}`);
});
