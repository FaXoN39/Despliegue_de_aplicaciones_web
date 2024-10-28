Ejercicio 4: Trait Loggable y Clase Producto
Descripción: Este ejercicio introduce el concepto de traits en PHP, permitiendo la reutilización de código entre diferentes clases.

Características:
Trait Loggable: Se crea un trait llamado Loggable que incluye un método log. Este método recibe un mensaje y lo imprime con una marca de tiempo.
Clase Producto: Se define una clase Producto que utiliza el trait Loggable.
Atributos: La clase tiene atributos privados como nombre y precio.
Métodos: Incluye un constructor para inicializar los atributos y un método setPrecio que permite modificar el precio del producto. Cada vez que se cambia el precio, se registra un mensaje mediante el método log.
