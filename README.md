<div align="center">
  
# BEPAFRANI || PABLO FERNÁNDEZ FERNÁNDEZ

</div>


# PRÁCTICA 2.2: Evaluación de IDEs

## 2.1. Instalación de entornos de desarrollo, propietarios y libres (CE 2.a)

Elige dos entornos de desarrollo: Instala ambos en tu equipo y captura pantallas del proceso de instalación.

**Preguntas evaluativas:**

1. **¿Qué diferencias encontraste en el proceso de instalación entre el IDE propietario y el libre?**

   Realmente en el proceso de instalación apenas hay diferencias, pero para PyCharm necesitas una clave, ya que es un software propietario. Si no, solo dispondrás de un periodo de 30 días; sin embargo, para VSCode solo necesitas entrar a la web e instalarlo.

2. **¿Qué ventajas identificaste en cada uno de los entornos durante la instalación?**

   Esto depende del usuario. VSCode es libre, por lo que es gratuito, lo que para algunos puede ser una ventaja. PyCharm es de pago, lo que para otros puede suponer una ventaja.

**Evidencia:** Captura de pantalla del proceso de instalación de cada IDE.

### PyCharm: Propietario

> [Instalación PyCharm](./Instalacion_PyCharm.pdf)

Cogemos la versión `windows.exe`, ARM es la versión móvil.

### Visual Studio CODE: Libre

> [Instalación Visual Studio Code](./Instalacion_VSCode.pdf)
---

## 2.2. Gestión de módulos y extensiones en el entorno de desarrollo (CE 2.b)

En cada IDE, agrega extensiones o módulos que amplíen su funcionalidad. Por ejemplo, instala una extensión para trabajar con Python en Visual Studio Code o un plugin para Kotlin en IntelliJ IDEA.

**Preguntas evaluativas:**

1. **¿Cómo fue el proceso de instalación de extensiones o módulos en cada IDE?**
> [Instalación Visual Studio Code](./Instalación_Extensiones.pdf)
2. **¿Qué beneficios proporcionan las extensiones o plugins que instalaste para el desarrollo de tus proyectos?**

**Evidencia:** Captura de pantalla del panel de extensiones o plugins instalados en cada IDE.

- **VSCode:** La instalación de las extensiones en Visual Studio es muy sencilla. Simplemente vamos a "Extensiones", seleccionamos la que queramos o la buscamos y la instalamos. Para Python usamos un conjunto de 3 extensiones, que son las siguientes:

> [Instalación Visual Studio Code](./Instalación_Extensiones_VSCode.pdf)

Por ejemplo, aquí se muestran las opciones que tienes con una extensión de Python. En el mismo sitio donde se ve "Uninstall", veríamos "Install"; simplemente es darle clic.

El beneficio que me permite es poder usar la extensión `.py`, básicamente, poder usar Python.

---

## 2.3. Personalización y automatización del entorno (CE 2.c)

### Tarea individual:
Personaliza el entorno de trabajo en cada IDE (tema, atajos de teclado) y automatiza una tarea, como la ejecución de pruebas o la compilación de código.

**Preguntas evaluativas:**

1. **¿Qué aspectos del entorno personalizaste y cómo mejoró tu experiencia de desarrollo?**

   Presionando `Ctrl + Shift + P` abrimos los comandos, ahí buscamos "color" y vamos a "Tema de colores" para elegir el que más nos guste. En mi caso lo dejé en negro, pero si lo ponemos en `light`, quedaría de esta manera:

> ![image](https://github.com/user-attachments/assets/be974625-39c6-442a-b124-a317f844b666)

2. **¿Cómo configuraste la automatización de tareas y en qué te benefició durante el trabajo?**

> ![image](https://github.com/user-attachments/assets/d5359771-8d15-46f1-8f1c-407f02fa4539)
> ![image](https://github.com/user-attachments/assets/bb7c1e7c-a72e-4dff-bc95-9c308a4108f9)
> ![image](https://github.com/user-attachments/assets/02117ee4-7665-462a-bb6b-68d9735731bf)

Este código nos compilará los archivos que se guarden directamente. Para ello necesitaremos la extensión "Run on Save".

> ![image](https://github.com/user-attachments/assets/7db3e11a-569f-4fca-85e9-28f4127f3cc8)

---

## 2.4. Configuración del sistema de actualización del entorno de desarrollo (CE 2.d)

### Tarea individual:
Configura el sistema de actualizaciones automáticas o manuales en ambos IDEs para asegurarte de que están al día con las últimas versiones y mejoras.

**Preguntas evaluativas:**

1. **¿Cómo configuraste las actualizaciones automáticas en cada IDE?**

   En `Settings`, tenemos que tener activada la opción de chequeo automático de actualizaciones, en `default`.

> ![image](https://github.com/user-attachments/assets/1ff83fc8-9ee0-4f3f-86dd-167d52c0776b)

2. **¿Por qué es importante mantener el IDE actualizado en proyectos de desarrollo?**

Mantener el IDE actualizado es importante para aprovechar las últimas características, mejoras de rendimiento y optimizaciones en el flujo de trabajo. Las actualizaciones también suelen tener correcciones de seguridad, reduciendo el riesgo de vulnerabilidades. Además, los cambios en los lenguajes y librerías de desarrollo se reflejan en los IDEs a través de actualizaciones, asegurando la compatibilidad con nuevas tecnologías y estándares.

**Evidencia:** Captura de pantalla de la configuración de actualizaciones en cada IDE.

> 
---

## 2.5. Generación de ejecutables a partir de código fuente en distintos lenguajes en un mismo IDE (CE 2.e)

### Tarea individual:
Escribe un programa que cuente de 10 a 0 y luego imprima "¡Despegue!". Usa un solo IDE para generar y ejecutar este programa en dos lenguajes diferentes (por ejemplo, Java y Kotlin en IntelliJ IDEA).

**Preguntas evaluativas:**

1. **¿Cuál fue el proceso para ejecutar el mismo programa en diferentes lenguajes dentro del mismo IDE?**
> ![image](https://github.com/user-attachments/assets/f55eee62-c125-45b0-bee6-deb468a2abbc)
> ![image](https://github.com/user-attachments/assets/c85300a5-9b18-4877-81f8-3fcd12b291c6)

2. **¿Qué diferencias encontraste en la generación del ejecutable entre los dos lenguajes?**

   Java es bastante diferente, se llama a la clase del nombre del archivo y no hay funciones, mientras que en Kotlin es similar a Python, aunque el código cambia un poco.

---

## 2.6. Generación de ejecutables con diferentes IDEs a partir del mismo código fuente (CE 2.f)

### Tarea individual:
Escribe un programa en Python que cuente de 10 a 0 y luego imprima "¡Despegue!". Ejecuta el programa en los IDEs seleccionados.

**Preguntas evaluativas:**

1. **¿Qué diferencias encontraste al ejecutar el mismo código fuente en diferentes IDEs?**

   IntelliJ es diferente; es más complejo y a su vez completo.

2. **¿Cuál de los IDEs te pareció más cómodo o eficiente para ejecutar el código Python o el lenguaje que hayas elegido? ¿Por qué?**

   Visual Studio Code, porque es el “IDE” con el que estoy acostumbrado a trabajar y es mucho más cómodo personalmente.
> ![image](https://github.com/user-attachments/assets/b9986ef4-b560-4dd6-9dac-1bcd9f133bcf)

---

