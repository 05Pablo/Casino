# Casino — Juegos clásicos en C++

## ¡Entra al casino, elige tu juego y pon a prueba tu suerte!

Aplicación de consola desarrollada en C++ que reúne diferentes juegos clásicos en una experiencia inspirada en un casino.

El proyecto permite crear usuarios, gestionar sus saldos y participar en distintos minijuegos, cada uno con sus propias reglas y mecánicas. Los jugadores pueden apostar, ganar o perder fondos y consultar su perfil.

## Juegos disponibles

El casino incluye ocho juegos:

| Juego | Descripción |
|---|---|
| **Piedra, papel o tijera** | Compite contra el sistema eligiendo piedra, papel o tijera. |
| **Tres en Raya** | Juega en un tablero de 3 × 3 contra una máquina que intenta bloquear tus jugadas ganadoras y realiza movimientos aleatorios. |
| **Wordle** | Intenta descubrir la palabra oculta mediante distintos intentos. |
| **Juego de los palillos** | Participa en el minijuego de los palillos. |
| **Tragaperras** | Prueba suerte intentando conseguir combinaciones ganadoras. |
| **Ruleta** | Realiza apuestas en el juego de la ruleta. |
| **Ahorcado** | Adivina una palabra letra a letra antes de agotar tus vidas. |
| **Blackjack** | Intenta acercarte a 21 puntos sin pasarte, jugando contra el croupier. |

## Gestión de usuarios

La aplicación dispone de un sistema de usuarios que permite:

- Registrarse con nombre, edad y saldo inicial.
- Iniciar sesión mediante un identificador.
- Consultar el saldo disponible.
- Añadir fondos y retirar dinero.
- Consultar estadísticas asociadas a los juegos.
- Eliminar usuarios registrados.

El sistema comprueba que los usuarios tengan al menos 18 años al registrarse.

## Sistema de apuestas

Los juegos incorporan un sistema de apuestas basado en el saldo del usuario.

Dependiendo del resultado de la partida, el jugador puede obtener ganancias, perder la cantidad apostada o recuperar su apuesta en caso de empate, según las reglas del juego.

## Organización del código

El proyecto está desarrollado de forma modular, separando las clases y la lógica de los juegos en archivos `.cpp` y `.hpp`.

- `Main.cpp`: punto de entrada de la aplicación.
- `Casino.cpp` y `Casino.hpp`: menús principales, acceso a los juegos y gestión de usuarios.
- `Usuario.cpp` y `Usuario.hpp`: información del usuario, saldo y estadísticas.
- `RegistroUsuario.cpp` y `RegistroUsuario.hpp`: operaciones relacionadas con el registro y almacenamiento de usuarios.
- Archivos específicos de cada juego: contienen sus reglas y mecánicas.
- `casino.txt` y `palabras_rae_l.txt`: archivos auxiliares utilizados por la aplicación.

## Requisitos

- Un compilador de C++ compatible con el código del proyecto, como **G++** o **MinGW**.
- Visual Studio Code u otro entorno de desarrollo compatible (opcional).
- Sistema operativo Windows recomendado, ya que el código utiliza funciones de consola propias de Windows, como `system("cls")` y `Sleep()`.

## Librerias
- iostream: entrada y salida por consola.

- string: manejo de cadenas de texto.

- vector: almacenamiento de colecciones de palabras.

- fstream: lectura y escritura de archivos.

- cstdlib y ctime: generación de números aleatorios y funciones auxiliares.

- stdexcept: gestión de excepciones.

