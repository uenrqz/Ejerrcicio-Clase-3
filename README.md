# Ejerrcicio-Clase-3
Ejercicio en conjunto con Yenci Hernamdez, Raquel Perez y Ulises Enriquez


Yenci Hernandez Deepseek:
Promt:
 
necesito que me ayudes con una estructura de datos, necesito que la puedas pasar a una cola

class cola {
constructor() {
this.items = [];
}

enqueue(element) {
this.items.push(element);
}

dequeue() {
if (this.isEmpty()) {
return "la cola esta vacia";
}
return this.items.shift();
}

frente() {
return this.items[0];
}

isEmpty() {
return this.items.length == 0;
}

mostrar() {
console.log(this.items);
}
}

//prueba cola
let miCola = new cola();
miCola.enqueue("Cliente 1");
miCola.enqueue("Cliente 2");
miCola.enqueue("Cliente 3");
miCola.mostrar(); // ["Cliente 1", "Cliente 2", "Cliente 3"]
console.log("atendiendo: " + miCola.dequeue()); // Cliente 1
console.log("siguiente en fila: " + miCola.frente()); // Cliente 2


siguiendo esto:

Especificaciones del tipo abstracto de datos Cola
Tipo de dato
Operaciones
Crear Cola
Insertar
Quitar
Cola vacía
Cola llena
Frente
Tamaño de la cola
Elemento que se almacena en la cola.
Inicia la cola como vacía.
Añade un elemento por el final de la cola.
Retira (extrae) el elemento frente de la cola.
Comprueba si la cola no tiene elementos.
Comprueba si la cola está llena de elementos.
Obtiene el elemento frente o primero de la cola.
Número de elementos máximo que puede contener la cola

Analisis utilizando Meta iA:

En mi experiencia, me mostro unicamente solo la difentecia entre una cola pura con una cola con arreglo, no mostrandome todo el codigo.


Raquel Perez Claude:

Crear Cola: Inicia la cola como vacía.
Insertar: Añade un elemento por el final de la cola.
Quitar: Retira (extrae) el elemento frente de la cola.
Cola vacía: Comprueba si la cola no tiene elementos.
Cola llena: Comprueba si la cola está llena de elementos.
Frente: Obtiene el elemento frente o primero de la cola.
Tamaño de la cola: Número de elementos máximo que puede contener la cola.
Elemento que se almacena en la cola: El tipo de dato que se almacena en la cola.
Requisitos adicionales:
Interacción con el usuario:
El programa debe pedir al usuario que ingrese la dimensión (tamaño máximo) de la cola que desea crear. Esta dimensión será utilizada para inicializar la cola.
Mensajes descriptivos:
Cada vez que se ejecute una operación (como insertar, quitar, verificar si está vacía, etc.), el programa debe imprimir un mensaje descriptivo que indique lo que está sucediendo. Por ejemplo:
Al insertar un elemento: "Se insertó el elemento [elemento] en la cola."
Al quitar un elemento: "Se retiró el elemento [elemento] de la cola."
Al verificar si la cola está vacía: "La cola está vacía." o "La cola no está vacía."
Al verificar si la cola está llena: "La cola está llena." o "La cola no está llena."
Al obtener el frente de la cola: "El elemento frente de la cola es [elemento]."
Al consultar el tamaño de la cola: "El tamaño máximo de la cola es [tamaño]."
Implementación de métodos:
Asegúrate de implementar todos los métodos mencionados en las especificaciones (Crear Cola, Insertar, Quitar, Cola vacía, Cola llena, Frente, Tamaño de la cola).
Cada método debe realizar la operación correspondiente y mostrar el mensaje descriptivo adecuado.
Manejo de errores:
Si el usuario intenta insertar un elemento en una cola llena, el programa debe mostrar un mensaje de error: "Error: La cola está llena, no se puede insertar más elementos."
Si el usuario intenta quitar un elemento de una cola vacía, el programa debe mostrar un mensaje de error: "Error: La cola está vacía, no se puede retirar ningún elemento."
Ejecución del programa:
El programa debe permitir al usuario interactuar con la cola mediante un menú o una serie de opciones que le permitan realizar las operaciones mencionadas (insertar, quitar, verificar si está vacía, etc.).
Después de cada operación, el programa debe mostrar el estado actual de la cola (por ejemplo, los elementos que contiene). Todo eso aplicalo a este código modificandolo con lo anterior mencionado, esto en entorno de node.js:






Ulises Enriquez Meta iA:

Promt:
 
necesito que me ayudes con una estructura de datos, necesito que la puedas pasar a una cola

class cola {
constructor() {
this.items = [];
}

enqueue(element) {
this.items.push(element);
}

dequeue() {
if (this.isEmpty()) {
return "la cola esta vacia";
}
return this.items.shift();
}

frente() {
return this.items[0];
}

isEmpty() {
return this.items.length == 0;
}

mostrar() {
console.log(this.items);
}
}

//prueba cola
let miCola = new cola();
miCola.enqueue("Cliente 1");
miCola.enqueue("Cliente 2");
miCola.enqueue("Cliente 3");
miCola.mostrar(); // ["Cliente 1", "Cliente 2", "Cliente 3"]
console.log("atendiendo: " + miCola.dequeue()); // Cliente 1
console.log("siguiente en fila: " + miCola.frente()); // Cliente 2


siguiendo esto:

Especificaciones del tipo abstracto de datos Cola
Tipo de dato
Operaciones
Crear Cola
Insertar
Quitar
Cola vacía
Cola llena
Frente
Tamaño de la cola
Elemento que se almacena en la cola.
Inicia la cola como vacía.
Añade un elemento por el final de la cola.
Retira (extrae) el elemento frente de la cola.
Comprueba si la cola no tiene elementos.
Comprueba si la cola está llena de elementos.
Obtiene el elemento frente o primero de la cola.
Número de elementos máximo que puede contener la cola

Analisis utilizando Meta iA:

En mi experiencia, me mostro unicamente solo la difentecia entre una cola pura con una cola con arreglo, no mostrandome todo el codigo. 

Comparativa:
En lo personal nos quedamos con Deepseek, por sus respuestas completas mientras que IA a Meta se queda muy corto con las explicaciones igual que Cladue.

