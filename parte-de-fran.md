# Práctica 2.2

## 2.1 Instalación de entornos de desarrollo, propietarios y libres

Elige dos entornos de desarrollo: Instala ambos en tu equipo y captura pantallas del proceso de instalación.

En mi caso, he elegido los IDEs **Visual Studio Code** y **IntelliJ IDEA**.

### Proceso de instalación:

**Visual Studio Code:**  
![Visual Studio Code - Imagen 1](./Capturas%20Fran/Visual%20Studio%20Code-1.png)  
![Visual Studio Code - Imagen 2](./Capturas%20Fran/Visual%20Studio%20Code-2.png)  
![Visual Studio Code - Imagen 3](./Capturas%20Fran/Visual%20Studio%20Code-3.png)  
![Visual Studio Code - Imagen 4](./Capturas%20Fran/Visual%20Studio%20Code-4.png)  
![Visual Studio Code - Imagen 5](./Capturas%20Fran/Visual%20Studio%20Code-5.png)  
![Visual Studio Code - Imagen 6](./Capturas%20Fran/Visual%20Studio%20Code-6.png)  
![Visual Studio Code - Imagen 7](./Capturas%20Fran/Visual%20Studio%20Code-7.png)  

**IntelliJ IDEA:**  
![IntelliJ IDEA - Imagen 1](./Capturas%20Fran/IntelliJ-1.png)  
![IntelliJ IDEA - Imagen 2](./Capturas%20Fran/IntelliJ-2.png)  
![IntelliJ IDEA - Imagen 3](./Capturas%20Fran/IntelliJ-3.png)  
![IntelliJ IDEA - Imagen 4](./Capturas%20Fran/IntelliJ-4.png)  
![IntelliJ IDEA - Imagen 5](./Capturas%20Fran/IntelliJ-5.png)  

### Preguntas evaluativas:

- **¿Qué diferencias encontraste en el proceso de instalación entre el IDE propietario y el libre?**

  Durante el proceso de instalación de ambos IDEs no he encontrado grandes diferencias. No obstante, sí durante el proceso de descarga del software. En el caso de **Visual Studio Code**, solo he necesitado entrar en la página de descarga (https://code.visualstudio.com/) y presionar el botón de descarga, obteniendo así el ejecutable.

  Por otro lado, en el caso de **IntelliJ IDEA**, he necesitado crear una cuenta en la web de JetBrains, usando mi correo electrónico institucional (@g.educaand.es) y así he conseguido una licencia temporal de un año.

  Una vez creada la cuenta, se procede de igual forma que con Visual Studio Code: descarga del ejecutable e instalación.

- **¿Qué ventajas identificaste en cada uno de los entornos durante la instalación?**

  Ambas instalaciones han sido prácticamente idénticas, más allá de la parte del registro, necesario en el caso de los IDEs publicados por JetBrains como IntelliJ IDEA.

  Además, en el caso de no disponer de una licencia de estudiante, sería necesario obtener una licencia de pago.

**Evidencia:** Captura de pantalla del proceso de instalación de cada IDE (ver capturas en Proceso de instalación).

## 2.2 Gestión de módulos y extensiones en el entorno de desarrollo

  En cada IDE, agrega extensiones o módulos que amplíen su funcionalidad. Por ejemplo, suponiendo habiendo trabajado con VSC y IntelliJ IDEA, instala una extensión para trabajar con Python en Visual Studio Code o un plugin para Kotlin en IntelliJ IDEA.

### Proceso de instalación de extensiones/plugins:

**Visual Studio Code:**  
![Visual Studio Code - Extensiones](./Capturas%20Fran/Visual%20Studio%20Code-instalacion-python.png)  

**IntelliJ IDEA:**  
![IntelliJ IDEA - Plugins](./Capturas%20Fran/Intellij-instalacion-python.png)

### Preguntas evaluativas:

- **¿Cómo fue el proceso de instalación de extensiones o módulos en cada IDE?**

  Mientras que **Visual Studio Code** tiene un apartado en el navegador lateral, junto a los iconos de Explorador, Buscar y Control de versiones, entre otros, que hace la instalación de extensiones especialmente intuitiva y fácil; en **IntelliJ IDEA** el proceso es un poco más complejo, ya que el menú de plugins (como es llamado en este caso) no está en la pantalla principal del programa, sino en el menú de opciones al que se accede desde File → Settings.

- **¿Qué beneficios proporcionan las extensiones o plugins que instalaste para el desarrollo de tus proyectos?**

  Instalar plugins o extensiones en los IDE proporciona características adicionales que facilitan el desarrollo, como funciones de autocompletado y sugerencias de código, depuración (lo que nos permite ejecutar el código paso a paso y analizar variables en tiempo real), testing (como pytest) y control de versiones. Gracias a esto, se consigue una mejora en la productividad.

**Evidencia:** Captura de pantalla del panel de extensiones o plugins instalados en cada IDE.

## 2.3 Personalización y automatización del entorno

Personaliza el entorno de trabajo en cada IDE (tema, atajos de teclado) y automatiza una tarea, como la ejecución de pruebas o la compilación de código.

### Preguntas evaluativas:

- **¿Qué aspectos del entorno personalizaste y cómo mejoró tu experiencia de desarrollo?**

  En **Visual Studio Code** he modificado el tema de la interfaz, eligiendo un tono más oscuro al que viene por defecto desde File → Preferences → Theme. Con esto se consigue reducir sustancialmente la fatiga visual que provoca estar expuesto a la pantalla durante sesiones de trabajo largas.
  En **IntelliJ IDEA** he creado un atajo o shortcut para duplicar líneas completas. En este caso, he tenido que abrir la ventana de Settings y hacerlo desde el apartado Keymap. Al configurar atajos de teclado, se reduce la utilización del ratón y, por tanto, se evitan las distracciones de cambiar del teclado al ratón. En el caso de trabajar con varios IDEs diferentes, al utilizar atajos similares, se consigue una mejora en la consistencia y rapidez en el flujo de trabajo.

  **En Visual Studio Code:**  
  ![Tema oscuro en VS Code](./Capturas%20Fran/Visual%20Studio%20Code-configuracion.png)

  **En IntelliJ IDEA:**  
  ![Atajo de teclado en IntelliJ IDEA](./Capturas%20Fran/IntelliJ-configuracion-shortcuts.png)

- **¿Cómo configuraste la automatización de tareas y en qué te benefició durante el trabajo?**

    En VS Code se configuran las tareas a través del menú Terminal → Configure Tasks → Create tasks.json from template. Tras esto, se configura la tarea a automatizar en el archivo tasks.json (por ejemplo, ejecutar pruebas con pytest):

  ```json
  {
    "version": "2.0.0",
    "tasks": [
      {
        "label": "run pytest",
        "type": "shell",
        "command": "pytest",
        "group": {
          "kind": "test",
          "isDefault": true
        },
        "problemMatcher": [],
        "runOptions": {
          "runOn": "fileSave"   // Ejecuta al guardar
        }
      }
    ]
  }
  ```
  
  ![Ejecución en IntelliJ IDEA](./Capturas%20Fran/Visual%20Studio%20Code-tarea.png)
  ![Ejecución en IntelliJ IDEA](./Capturas%20Fran/Visual%20Studio%20Code-ejecucion-tarea.png)

    En IntelliJ IDEA he decidido automatizar la compilación de los proyectos cada vez que este se guarda. Para ello, es necesario ir a File → Settings → Build, Execution, Deployment → Compiler. Aquí, marco la opción Build project automatically.
  
  ![Ejecución en IntelliJ IDEA](./Capturas%20Fran/IntelliJ-tarea.png)

## 2.4 Configuración del sistema de actualización del entorno de desarrollo

  Configura el sistema de actualizaciones automáticas o manuales en ambos IDEs para asegurarte de que están al día con las últimas versiones y mejoras.

### Preguntas evaluativas:

- **¿Cómo configuraste las actualizaciones automáticas en cada IDE?**

    En **Visual Studio Code**, el modo en que se gestionan las actualizaciones se configura desde File → Preferences → Settings → ‘update’ (en el buscador). Se puede ejecutar en los modos None, Manual, Start y Default.

  ![Configuración de actualizaciones en VS Code](./Capturas%20Fran/Visual%20Studio%20Code-updates.png)

    En **IntelliJ IDEA** se hace de manera muy similar, navegando a File → Settings → System Setting → Updates

  ![Configuración de actualizaciones en IntelliJ IDEA](./Capturas%20Fran/IntelliJ-updates.png)

- **¿Por qué es importante mantener el IDE actualizado en proyectos de desarrollo?**

  Mantener el IDE actualizado nos permite aprovechar al máximo las mejoras de rendimiento, características añadidas en las nuevas versiones, compatibilidad con las últimas tecnologías, corrección de error y posibles vulnerabilidades de seguridad y, en general, mejorar la experiencia de desarrollo.

**Evidencia:** Captura de pantalla de la configuración de actualizaciones en cada IDE.

## 2.5 Generación de ejecutables a partir de código fuente en distintos lenguajes en un mismo IDE

Escribe un programa que cuente de 10 a 0 y luego imprima "¡Despegue!". Usa un solo IDE para generar y ejecutar este programa en dos lenguajes diferentes (por ejemplo, Java y Kotlin en IntelliJ IDEA).

### Preguntas evaluativas:

- **¿Cuál fue el proceso para ejecutar el mismo programa en diferentes lenguajes dentro del mismo IDE?**

  - **Java en IntelliJ IDEA:**
  Para ejecutar el programa en Java dentro de **IntelliJ IDEA**, primero creé un proyecto de tipo Java y luego añadí un archivo de clase llamado Countdown.java. Escribí el código en Java que contaba de 10 a 0 usando un bucle for. Una vez que el código estuvo listo, verifiqué que el proyecto tuviera un JDK configurado correctamente. Luego, simplemente hice clic derecho en el archivo y seleccioné Run Countdown.main() para ejecutar el programa.

    ![Ejecución en Java](./Capturas%20Fran/Java-programa.png)

  - **Kotlin en IntelliJ IDEA:**
    Para ejecutar el mismo programa en **Kotlin**, creé un archivo nuevo llamado Countdown.kt dentro del mismo proyecto en IntelliJ IDEA. Escribí el código en Kotlin, que utiliza la función downTo para contar de 10 a 0. Comprobé que el proyecto estuviera configurado para soportar Kotlin. Después de crear el archivo Kotlin, hice clic derecho sobre él y seleccioné Run Countdown.main(). Al ejecutar el programa, obtuve el mismo resultado que en Java, pero ahora usando Kotlin.

    ![Ejecución en Kotlin](./Capturas%20Fran/Kotlin-programa.png)

- **¿Qué diferencias encontraste en la generación del ejecutable entre los dos lenguajes?**

  La diferencia principal al generar el ejecutable entre **Java y Kotlin** es que, aunque ambos lenguajes terminan en un formato que puede ser ejecutado por la JVM (Java Virtual Machine), el proceso es ligeramente diferente. En Java, primero se compila el código en archivos .class, que luego se ejecutan. En Kotlin, el proceso es más directo, ya que se integra de manera más fluida en IntelliJ IDEA, y el código se compila automáticamente para ser ejecutado. Sin embargo, ambos lenguajes requieren la JVM para ejecutar el programa, por lo que, en la práctica, el resultado final es bastante similar.

**Evidencia:** Captura de pantalla mostrando la ejecución del programa en ambos lenguajes dentro del mismo IDE.

## 2.6 Generación de ejecutables con diferentes IDEs a partir del mismo código fuente

Escribe un programa en Python que cuente de 10 a 0 y luego imprima "¡Despegue!". Ejecuta el programa en los IDEs seleccionados.

- **En Visual Studio Code:**
  
  ![Ejecución en Visual Studio Code](./Capturas%20Fran/Visual%20Studio%20Code-python-programa.png)

- **En IntelliJ IDEA:**
  
  ![Ejecución en IntelliJ IDEA](./Capturas%20Fran/IntelliJ-python-programa.png)

### Preguntas evaluativas:

- **¿Qué diferencias encontraste al ejecutar el mismo código fuente en diferentes IDEs?**

  A grandes rasgos, el proceso fue muy similar en ambos entornos. Ambos IDEs requieren configurar el intérprete de Python y ejecutar el código con unos pocos clics. La diferencia principal es que **IntelliJ IDEA** tiene una interfaz más completa y estructurada, mientras que **VS Code** es más ligero y rápido de configurar, pero ambos ofrecen una experiencia similar para ejecutar programas pequeños.

- **¿Cuál de los IDEs te pareció más cómodo o eficiente para ejecutar el código Python o el lenguaje que hayas elegido? ¿Por qué?**

  Prefiero **Visual Studio Code**. Mi primera impresión como usuario de **IntelliJ IDEA** es que se trata de un IDE más completo y potente que VS Code, pero a la vez más complejo de configurar y utilizar en general. Aunque ambas interfaces son muy parecidas, Visual Studio Code muestra de una forma más explícita qué es  cada elemento (como en el panel lateral), sin necesidad de abrir menús previamente. Esto hace que, para alguien que se está introduciendo en la programación, sea mucho más intuitivo reconocer las características disponibles.

**Evidencia:** Captura de pantalla mostrando la ejecución del programa en ambos IDEs.
