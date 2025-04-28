# TallerPD

-------------------

CREATE DATABASE usuarios;

USE usuarios;

CREATE TABLE personas (
    id INT AUTO_INCREMENT PRIMARY KEY,
    nombre VARCHAR(50),
    apellido VARCHAR(50),
    edad INT
);


----------------------
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <title>Formulario de Usuarios</title>
</head>
<body>
    <h2>Agregar Persona</h2>
    <form action="insertar.php" method="POST">
        Nombre: <input type="text" name="nombre" required><br>
        Apellido: <input type="text" name="apellido" required><br>
        Edad: <input type="number" name="edad" required><br>
        <input type="submit" value="Guardar">
    </form>

    <h2>Buscar Persona por Nombre</h2>
    <form action="buscar.php" method="GET">
        Nombre: <input type="text" name="nombre" required>
        <input type="submit" value="Buscar">
    </form>
</body>
</html>


