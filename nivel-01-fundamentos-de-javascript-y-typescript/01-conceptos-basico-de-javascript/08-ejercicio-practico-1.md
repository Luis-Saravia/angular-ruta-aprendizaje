**Ejercicio Práctico: Calculadora de Suma y Promedio**

**Descripción:** Escribe un programa en JavaScript que permita al usuario ingresar una serie de números y luego calcule la suma y el promedio de esos números.

**Pasos a seguir:**

1. Solicitar al usuario la cantidad de números que desea ingresar.
2. Usar un bucle para iterar y pedir al usuario que ingrese cada número.
3. Almacenar los números en una matriz o lista.
4. Calcular la suma de todos los números.
5. Calcular el promedio dividiendo la suma entre la cantidad de números.
6. Mostrar los resultados al usuario.

```javascript
// Solicitar al usuario la cantidad de números a ingresar
var cantidadNumeros = parseInt(prompt("Ingrese la cantidad de números:"));

// Inicializar la suma en cero
var suma = 0;

// Crear una lista para almacenar los números
var numeros = [];

// Iterar para pedir al usuario que ingrese los números
for (var i = 0; i < cantidadNumeros; i++) {
  var numero = parseFloat(prompt("Ingrese el número " + (i + 1) + ":"));
  numeros.push(numero); // Agregar el número a la lista
  suma += numero; // Sumar el número a la suma total
}

// Calcular el promedio dividiendo la suma entre la cantidad de números
var promedio = suma / cantidadNumeros;

// Mostrar los resultados al usuario
console.log("Números ingresados:", numeros);
console.log("Suma total:", suma);
console.log("Promedio:", promedio);
```

**Ejemplo de uso:**

Supongamos que el usuario ingresa que desea ingresar 4 números: 10, 15, 5 y 8. El programa calcularía lo siguiente:

```
Números ingresados: [10, 15, 5, 8]
Suma total: 38
Promedio: 9.5
```

Este ejercicio práctico te permite aplicar los conceptos de variables, bucles y condicionales para resolver un problema específico. A medida que avanzas en tu aprendizaje, podrás enfrentar desafíos más complejos y aplicar estos fundamentos en situaciones más elaboradas, incluyendo el desarrollo de aplicaciones web con Angular. ¡Sigue practicando y construyendo tu confianza en JavaScript!