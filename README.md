# Despliegue_de_aplicaciones_web
ReadME de los ejercicios:
Ejercicio3:
Primero nos dirigiremos al moodle de esemtia y antes de iniciar sesion abriremos la consola y nos dirigiremos a la pestaña de Network.
Capturaremos el tráfico al iniciar sesión en Moodle, al iniciar sesión con la consola abierta veremos las peticiones.
Una vez realizado el inicio de sesión y de ver todas las peticiones buscaremos la petición POST que es la que nos interesa para el tema de las credenciales.
![image](https://github.com/user-attachments/assets/ec2446b1-d792-495f-8f1f-fcb0ed87a501)
Encontraremos lo que nos interesa en la primera petición que se llama index.php y en el apartado PayLoad encontraremos, en mi caso, mi credencial del Moodle y el loginToken.
![image](https://github.com/user-attachments/assets/5eae7a56-2f2d-4fd1-bd01-7b9281174eae)
Los datos sensibles salen del Usuario y Contraseña, donde estos datos se ingresan manualmente en el formulario de inicio de sesión. Son capturados en el navegador y enviados al servidor en la petición POST.
Despues tenemos el token CSRF, este token es generado por el servidor antes de que el usuario envié el formulario. Normalmente se incluye como un campo oculto en el formulario HTML, y se envía junto con la petición de inicio de sesión para asegurar que la petición sea legítima.
Por último tenemos el token de sesión dónde el servidor genera el token de sesión y lo envía en una cookie. Este token es almacenado en el navegador y se incluye automáticamente en las peticiones posteriores al servidor, identificando la sesión activa.

Ejercicio4:
También localizaremos los headers y los datos enviados al lado de la pestaña de PayLoad.
![image](https://github.com/user-attachments/assets/535aec2a-68f5-49d9-9f99-f48adafd84ad)
Las peticiones del protocolo HTTP se reciben normalmente en el puerto 80. Este es el puerto estandar utilzado para la comunnicación web no segura (HTTP).
El modelo TCP/IP se encuentra en la capa de aplicación del protocolo HTTP, es la más alta de las cuatro capas del modelo TCP/IP.
Las otras capas son las siguientes:
-Capa de transporte. En esta se encuentra el protoclo TCP y el protocolo UDP.
-Capa de internet. En esta capa se encuentra el protocolo IP.
-Capa de enlace de Datos (Acceso a la red).

Ejercicio5:
![image](https://github.com/user-attachments/assets/81cc40d1-5ff1-4407-ad8f-28cf9075c099)
La respuesta del servidor HTTP/1.1 302 Found indica que la solicitud se ha procesado correctamente, pero que el recurso solicitado se ha movido temporalmente a otra ubicación.

Ejercicio6:
No es posible realizar el ejercicio debido a la falta de credenciales para instalar el programa de WireShark.
