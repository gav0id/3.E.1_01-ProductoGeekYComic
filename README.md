Ejercicio 3.E.1 01 - ProductoGeek y Comic

Lógica del programa
Para dar inicio a este nuevo bloque sobre Herencia, trabajé en la creación de una jerarquía de clases básica. Primero, diseñé la superclase `ProductoGeek` definiendo sus atributos `codigo`, `nombre` y `precioBase` con el modificador de acceso `protected`. La elección de este modificador es fundamental en la herencia, ya que permite que las clases hijas puedan heredar y manipular esta información internamente, algo que `private` bloquearía.

Luego, desarrollé la subclase `Comic`. Para establecer la relación de herencia, utilicé la palabra clave `extends ProductoGeek`. A esta nueva clase le agregué un atributo específico y privado: `numeroTomo` (int). 

El punto clave de este ejercicio fue la implementación del constructor de la subclase. En lugar de inicializar los atributos heredados de forma manual y duplicar código, utilicé la instrucción `super(codigo, nombre, precioBase)` en la primera línea del constructor. Esto me permitió delegar esa tarea directamente al constructor de la superclase.

Finalmente, en la clase `Main`, implementé la lógica de prueba:
1. Instancié un objeto `Comic` pasándole todos los parámetros necesarios (los heredados y los propios).
2. A través de las impresiones por consola, demostré que este objeto no solo posee su propio método `getNumeroTomo()`, sino que también heredó exitosamente los comportamientos `getNombre()` y `getPrecioBase()` de su clase padre, pudiendo utilizarlos como si hubieran sido definidos en su misma clase.

Ejecución en consola
<img width="1917" height="1018" alt="image" src="https://github.com/user-attachments/assets/ccce0f00-efed-4f26-bddf-c8de914821ce" />
