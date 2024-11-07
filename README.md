<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Tienda de Decants de Perfumes</title>
  <link rel="stylesheet" href="styles.css">
  <script src="scripts.js" defer></script>
</head>
<body>
  <header>
    <nav>
      <ul>
        <li><a href="#invierno">Perfumes de Invierno</a></li>
        <li><a href="#verano">Perfumes de Verano</a></li>
        <li><a href="#primavera">Perfumes de Primavera</a></li>
        <li><a href="#otono">Perfumes de Otoño</a></li>
      </ul>
    </nav>
    <h1>Bienvenidos a nuestra Tienda de Decants</h1>
  </header>

  <main>
    <!-- Sección de Invierno -->
    <section id="invierno">
      <h2>Perfumes de Invierno</h2>
      <div class="perfume">
        <h3>Perfume 1</h3>
        <p>Descripción del perfume de invierno 1.</p>
        <label for="invierno1">Selecciona el tamaño:</label>
        <select id="invierno1" class="tamaño">
          <option value="2ml">2ml</option>
          <option value="5ml">5ml</option>
          <option value="10ml">10ml</option>
        </select>
      </div>
    </section>

    <!-- Sección de Verano -->
    <section id="verano">
      <h2>Perfumes de Verano</h2>
      <div class="perfume">
        <h3>Perfume 2</h3>
        <p>Descripción del perfume de verano 2.</p>
        <label for="verano1">Selecciona el tamaño:</label>
        <select id="verano1" class="tamaño">
          <option value="2ml">2ml</option>
          <option value="5ml">5ml</option>
          <option value="10ml">10ml</option>
        </select>
      </div>
    </section>

    <!-- Sección de Primavera -->
    <section id="primavera">
      <h2>Perfumes de Primavera</h2>
      <div class="perfume">
        <h3>Perfume 3</h3>
        <p>Descripción del perfume de primavera 3.</p>
        <label for="primavera1">Selecciona el tamaño:</label>
        <select id="primavera1" class="tamaño">
          <option value="2ml">2ml</option>
          <option value="5ml">5ml</option>
          <option value="10ml">10ml</option>
        </select>
      </div>
    </section>

    <!-- Sección de Otoño -->
    <section id="otono">
      <h2>Perfumes de Otoño</h2>
      <div class="perfume">
        <h3>Perfume 4</h3>
        <p>Descripción del perfume de otoño 4.</p>
        <label for="otono1">Selecciona el tamaño:</label>
        <select id="otono1" class="tamaño">
          <option value="2ml">2ml</option>
          <option value="5ml">5ml</option>
          <option value="10ml">10ml</option>
        </select>
      </div>
    </section>

  </main>

  <footer>
    <p>&copy; 2024 Tienda de Decants de Perfumes. Todos los derechos reservados.</p>
  </footer>
</body>
</html>
body {
  font-family: Arial, sans-serif;
  margin: 0;
  padding: 0;
  background-color: #f4f4f4;
}

header {
  background-color: #333;
  color: white;
  padding: 10px 0;
  text-align: center;
}

header nav ul {
  list-style-type: none;
  padding: 0;
}

header nav ul li {
  display: inline;
  margin: 0 20px;
}

header nav ul li a {
  color: white;
  text-decoration: none;
}

h1 {
  margin: 0;
}

main {
  padding: 20px;
}

section {
  margin: 20px 0;
}

.perfume {
  background-color: white;
  padding: 15px;
  margin: 10px 0;
  border: 1px solid #ccc;
}

.perfume select {
  margin-top: 10px;
  padding: 5px;
}

footer {
  text-align: center;
  padding: 10px;
  background-color: #333;
  color: white;
}
// Este script puede ser expandido con funciones para agregar productos al carrito y calcular el precio final, entre otras características.

document.addEventListener("DOMContentLoaded", () => {
  // Aquí puedes agregar funcionalidades adicionales como el cálculo de precio o agregar al carrito
  const selects = document.querySelectorAll('.tamaño');
  selects.forEach(select => {
    select.addEventListener('change', (event) => {
      alert(`Has seleccionado el tamaño ${event.target.value}`);
    });
  });
});
