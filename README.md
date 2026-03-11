# Dropper

## Descripción

**Drop Catcher** es un juego **2D arcade** en el que el jugador controla un cubo que debe moverse por la parte inferior de la pantalla para **atrapar gotas que caen desde la parte superior**.
El objetivo es recoger el mayor número de gotas posible antes de quedarse sin vidas.

El juego incluye un **sistema de vidas**, por lo que cada vez que una gota cae al suelo sin ser atrapada el jugador pierde una vida. Cuando las vidas llegan a cero, la partida termina y se muestra la pantalla de **Game Over**.

Este proyecto está desarrollado con **Java** utilizando el framework **libGDX**, lo que permite ejecutarlo tanto en **ordenadores** como en **dispositivos Android**.

---

## Características

* Juego **2D estilo arcade**.
* Sistema de **puntuación** basado en gotas recogidas.
* **Sistema de vidas** (pierdes una vida cuando una gota cae al suelo).
* Pantalla de **Game Over** al quedarse sin vidas.
* **Música y efectos de sonido**.
* Compatible con **PC y Android**.
* Control mediante **teclado o pantalla táctil**.

---

## Cómo jugar

### Objetivo

Atrapar todas las gotas posibles con el cubo antes de quedarte sin vidas.

### Controles

**En ordenador**

* `←` Mover el cubo a la izquierda
* `→` Mover el cubo a la derecha

**En Android**

* Tocar la pantalla para mover el cubo hacia la posición del dedo.

### Mecánica

* Cada gota atrapada aumenta la puntuación.
* Si una gota cae al suelo se pierde **una vida**.
* El juego termina cuando el jugador pierde todas sus vidas.

---

## Tecnologías utilizadas

* **Java**
* **libGDX**
* **Gradle**
* **Android SDK**

---

## Estructura del proyecto

```
project-root
│
├── core
│   ├── GameScreen.java
│   └── lógica principal del juego
│
├── desktop
│   └── launcher para PC
│
├── android
│   └── versión para dispositivos móviles
│
└── assets
    ├── background.png
    ├── bucket.png
    ├── drop.png
    ├── music.mp3
    └── drop.mp3
```

---

```bash

```

### Ejecutar en ordenador

Ejecutar el launcher de escritorio desde el módulo **desktop**.

### Ejecutar en Android

Abrir el proyecto en **Android Studio** y ejecutar el módulo **android** en un dispositivo o emulador.

---

---

## Autor

Proyecto desarrollado por **Alejandro Guzman**.




# Droper

A [libGDX](https://libgdx.com/) project generated with [gdx-liftoff](https://github.com/libgdx/gdx-liftoff).

This project was generated with a template including simple application launchers and an `ApplicationAdapter` extension that draws libGDX logo.

## Platforms

- `core`: Main module with the application logic shared by all platforms.
- `lwjgl3`: Primary desktop platform using LWJGL3; was called 'desktop' in older docs.
- `android`: Android mobile platform. Needs Android SDK.

## Gradle

This project uses [Gradle](https://gradle.org/) to manage dependencies.
The Gradle wrapper was included, so you can run Gradle tasks using `gradlew.bat` or `./gradlew` commands.
Useful Gradle tasks and flags:

- `--continue`: when using this flag, errors will not stop the tasks from running.
- `--daemon`: thanks to this flag, Gradle daemon will be used to run chosen tasks.
- `--offline`: when using this flag, cached dependency archives will be used.
- `--refresh-dependencies`: this flag forces validation of all dependencies. Useful for snapshot versions.
- `android:lint`: performs Android project validation.
- `build`: builds sources and archives of every project.
- `cleanEclipse`: removes Eclipse project data.
- `cleanIdea`: removes IntelliJ project data.
- `clean`: removes `build` folders, which store compiled classes and built archives.
- `eclipse`: generates Eclipse project data.
- `idea`: generates IntelliJ project data.
- `lwjgl3:jar`: builds application's runnable jar, which can be found at `lwjgl3/build/libs`.
- `lwjgl3:run`: starts the application.
- `test`: runs unit tests (if any).

Note that most tasks that are not specific to a single project can be run with `name:` prefix, where the `name` should be replaced with the ID of a specific project.
For example, `core:clean` removes `build` folder only from the `core` project.
