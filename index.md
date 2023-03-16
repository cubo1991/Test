let sum = 'SUMA'
let rest = 'RESTA'
let mult = 'MULTIPLICACION'
let div = 'DIVISION'


// Ejercicio 1
for (let i = 100; i < 150; i++) {
    if(i%2 ===1) {
      return console.logi
    }
    ;
  }

// Ejercicio 2

<!DOCTYPE html>
<html>
  <head>
    <title>Calculadora</title>
    
  </head>
  <body>
    <h1>Calculadora</h1>
    <label for="a">Ingrese el valor de a:</label>
    <input type="number" id="a"><br><br>
    <label for="b">Ingrese el valor de b:</label>
    <input type="number" id="b"><br><br>
    <label for="operacion">Seleccione la operación:</label>
    <select id="operacion">
      <option value="sum">Suma</option>
      <option value="rest">Resta</option>
      <option value="mult">Multiplicación</option>
      <option value="div">División</option>
    </select><br><br>
    <button onclick="calcular()">Calcular</button><br><br>
    <div id="resultado"></div>

    <script>
         function calcular() {
    const a = parseFloat(document.getElementById("a").value);
    const b = parseFloat(document.getElementById("b").value);
    const operacion = document.getElementById("operacion").value;
    const resultado = calculadora(operacion, a, b);
    document.getElementById("resultado").innerHTML = resultado;
    console.log("Funciona")
  }

  let calculadora = (operacion, a, b ) => {
    if(Number.isInteger(a) && Number.isInteger(b)){
       if(operacion === 'sum') {return a+b}
       else if(operacion === 'rest') {return a-b}
       else if(operacion === 'mult') {return a*b}
       else if(operacion === 'div') {return a/b} 
       else {return 'Ingrese una operación válida'}
    } else{ console.log("Uno de los valores no es entero")
return 'Uno de los valores no es entero'}
  }
    </script>
    <script>
        
    </script>
  </body>
</html>

//Ejercicio3

HTML significa "Hypertext Markup Language" o "Lenguaje de Marcado de Hipertexto" en español. Es el lenguaje utilizado para crear páginas web y describe la estructura y contenido de una página web.
Su estructura básica contiene: las etiquetas html, head, y body. Además hay otras etiquetas que ayudan a marcar y ordenar el contenido de la página. 

  
  //Ejercicio 4
  let vehiculo = [{"color": "rojo","marca": "bmw","capacidad": 11},{"color": "azul","marca": "fiat","capacidad": 2},{"color": "negro","marca": "hyundai","capacidad": 6},{"color": "amarillo","marca": "jeep","capacidad": 15},{"color": "azul","marca": "citroen","capacidad": 20},{"color": "azul","marca": "renault","capacidad": 12},{"color": "rojo","marca": "ford","capacidad": 4},{"color": "gris","marca": "toyota","capacidad": 8}];

  let vehiculosFilter = vehiculo.filter( vehiculo => vehiculo.color === "azul" && vehiculo.capacidad > 10)
  console.log(vehiculosFilter)




