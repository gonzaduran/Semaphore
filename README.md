Aparcamiento Concurrente con Semaphore

Este programa simula un aparcamiento con 3 plazas al que intentan acceder 7 coches (hilos) al mismo tiempo.
Se utiliza la clase Semaphore de Java para controlar cuántos coches pueden aparcar simultáneamente y evitar conflictos de concurrencia.

⚙️ Funcionamiento

Solo 3 coches pueden estar dentro del aparcamiento.

Cuando está lleno, los demás esperan hasta que se libere una plaza.

Cada coche ocupa una plaza durante un tiempo aleatorio entre 1 y 4 segundos.

El programa muestra por consola qué coche entra, sale y el número de plazas ocupadas.

Ejemplo:

Coche-1 ha entrado. Plazas ocupadas: 1/3
Coche-2 ha entrado. Plazas ocupadas: 2/3
Coche-3 ha entrado. Plazas ocupadas: 3/3
Coche-1 ha salido. Plazas ocupadas: 2/3

🧩 Estructura
Aparcamiento.java   → Controla las plazas (Semaphore)
Coche.java          → Representa cada coche (hilo)
PrincipalParking.java → Lanza los hilos

🧠 Conclusión

El Semaphore permite limitar el acceso concurrente a un recurso compartido, evitando que más de 3 coches entren al mismo tiempo.
Cada ejecución puede mostrar un orden distinto, lo que demuestra el comportamiento no determinista de los hilos.

Autor: Gonzalo Durán Parreño
Fecha: 10/11/2025
Asignatura: Programación de Servicios y Procesos – Tema 6
