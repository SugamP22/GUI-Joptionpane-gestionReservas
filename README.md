# GUI-Joptionpane-gestionReservas

Este es un programa en Java que simula la gestión de reservas de hotel. Permite añadir, cancelar y mostrar reservas de habitaciones para los huéspedes. La interfaz de usuario se gestiona mediante ventanas emergentes (JOptionPane) y las reservas se almacenan en un conjunto (HashSet).

Funcionalidades
El programa cuenta con un menú interactivo con las siguientes opciones:

Añadir reserva: Permite añadir una nueva reserva para un huésped, con la opción de elegir el tipo de habitación (SIMPLE, DOUBLE, o SUITE), fecha de entrada y fecha de salida.

Cancelar reserva: Permite cancelar una reserva seleccionando el ID del huésped y la habitación.

Mostrar reservas: Muestra todas las reservas actuales.

Salir: Cierra el programa.

Estructura del código
Clases principales
GestionDeReservas: Es la clase principal que gestiona la interacción con el usuario, mostrando el menú, capturando las opciones seleccionadas y llamando a los métodos correspondientes para manejar las reservas.

Reservas: Representa una reserva en el hotel. Contiene información sobre el huésped, la habitación y las fechas de entrada y salida.

Habitaciones: Representa una habitación del hotel, con un tipo (SIMPLE, DOUBLE o SUITE).

Huespedes: Representa a un huésped, con su nombre, ID y preferencia.

Tipo: Enum que define los tipos de habitaciones disponibles: SIMPLE, DOUBLE y SUITE.

Funciones principales
aniadirReserva(): Permite al usuario añadir una nueva reserva proporcionando detalles como el nombre del huésped, el ID, la preferencia y el tipo de habitación. También solicita las fechas de entrada y salida.

cancelarReserva(): Permite al usuario cancelar una reserva existente mediante la introducción de los ID del huésped y de la habitación.

mostrarReserva(): Muestra todas las reservas existentes en el sistema.

Manejo de errores
El programa maneja excepciones como la introducción de datos inválidos o duplicados, y muestra mensajes de error utilizando JOptionPane.

Si se intenta cancelar una reserva que no existe, se muestra un mensaje de error.
