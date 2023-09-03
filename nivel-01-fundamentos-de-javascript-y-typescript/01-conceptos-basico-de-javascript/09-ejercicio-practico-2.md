**Ejercicio Práctico: Realizar Pruebas y Ajustes**

**Descripción:** Después de escribir el programa que calcula la suma y el promedio de números ingresados por el usuario, realizaremos pruebas y haremos ajustes para comprender cómo fluye la ejecución del programa y cómo se comporta en diferentes situaciones.

**Pasos a seguir:**

1. Ejecutar el programa con valores de muestra.
2. Observar y registrar los resultados.
3. Identificar posibles problemas o situaciones inesperadas.
4. Hacer ajustes en el código para abordar los problemas identificados.
5. Volver a ejecutar el programa y verificar los cambios.

**Código Original:**

```javascript
var cantidadNumeros = parseInt(prompt("Ingrese la cantidad de números:"));
var suma = 0;
var numeros = [];

for (var i = 0; i < cantidadNumeros; i++) {
  var numero = parseFloat(prompt("Ingrese el número " + (i + 1) + ":"));
  numeros.push(numero);
  suma += numero;
}

var promedio = suma / cantidadNumeros;

console.log("Números ingresados:", numeros);
console.log("Suma total:", suma);
console.log("Promedio:", promedio);
```

**Pruebas y Ajustes:**

1. Ejecutemos el programa con valores de muestra: ingresaremos los números 5, 7 y 3.

2. Observemos los resultados y registremos las salidas:

   ```
   Números ingresados: [5, 7, 3]
   Suma total: 15
   Promedio: 5
   ```

3. Identifiquemos problemas potenciales:

   - El promedio calculado parece incorrecto.
   - El promedio debería ser (5 + 7 + 3) / 3 = 5.

4. Realicemos un ajuste en el código para corregir el cálculo del promedio:

   ```javascript
   // Calcular el promedio dividiendo la suma entre la cantidad de números
   var promedio = suma / numeros.length; // Usar .length en lugar de cantidadNumeros
   ```

5. Ejecutemos el programa nuevamente con los mismos valores de muestra y verifiquemos si el ajuste resuelve el problema:

   ```
   Números ingresados: [5, 7, 3]
   Suma total: 15
   Promedio: 5
   ```

¡Excelente! Hemos realizado una prueba, identificado un problema y ajustado el código para solucionarlo. Este proceso es esencial para comprender cómo funciona el flujo de ejecución del programa y cómo responderá ante diferentes situaciones. Continuar practicando pruebas y ajustes te ayudará a desarrollar habilidades de depuración y a mejorar tus capacidades de programación en general.