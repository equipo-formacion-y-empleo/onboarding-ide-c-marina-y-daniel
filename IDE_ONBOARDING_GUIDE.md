# Guía de Configuración de Entornos de Desarrollo

> 📋 **Guía Técnica**: Esta documentación establece los procedimientos para configurar un entorno de desarrollo en C# y otros lenguajes. Incluye las configuraciones necesarias para mantener consistencia en el desarrollo de software.

> **Nota importante**: Este documento se enfoca en aspectos técnicos y procedimientos. Para análisis comparativos, reflexiones personales y conclusiones, utiliza el archivo `CONCLUSIONES_EVALUACION.md`.

**Autores**: Daniel y Marina
**Fecha V0**: 08/11/2025
**Fecha V1**: [Fecha de entrega final]

---

## Visual Studio Code - Entorno Principal

### Instalación y Verificación

**Método de instalación:** [desde la pagina web oficial de Visual Studio Code ![https://code.visualstudio.com/](<Captura de pantalla 2025-10-08 172620.png>)]

**Proceso de instalación:**
- **Descarga:** [Estando situados en la página de VS Code!
[https://code.visualstudio.com/download](<Captura de pantalla 2025-10-08 172558.png>) instalamos el paquete para windows, una vez descargado nos salen varias pestañas para seguir el proceso de descarga...]
- **Opciones del instalador:** [![instalamos el paquete para windows](<Captura de pantalla 2025-10-08 172546.png>); ![Una vez descargado le damos a "abrir archivo"](<Captura de pantalla 2025-10-08 174141.png>); ![Elegimos las funciones que queremos que tenga nuestro Visual Code en este caso"](<Captura de pantalla 2025-10-08 174740.png>); ![Esperamos a que el programa se instale](<Captura de pantalla 2025-10-08 174804.png>); ![Una vez instalamos, le damos Ejecutar Visual Studio Code](<Captura de pantalla 2025-10-08 174823.png>)]

- **Verificación:** [ ![Una vez instalado, nos adentramos a la aplicación, una vez metido nos sale todo el contenido y herraminetas que contiene el Visual](<Captura de pantalla 2025-10-10 174438.png>)]

*Es posible documentar múltiples métodos.*

### Uso Básico de VS Code

**Navegación y funcionalidades básicas:** 
- Navegación por la interfaz, Para poder navegar en VS, utilizaremos Ctrl + Tab, para cambiar de pestañas de archivos abiertos y Ctrl + P, para asi abrir un archivo del proyecto, tambien podemos utilizar Ctrl + G para ir a una linea especifica, 
- Edición de código, permite a los programadores escribir y editar un código fuente de una manera mas eficiente, la diferencia que tieen con un editor de texto, es que ofrece funciones especializadas como resalto de sintaxis 
- Uso de la paleta de comandos: si ponemos Ctrl + Mayús + P obtendremos el acceso a la paleta de comandos, una herramienta muyútil para encontrar funciones y configuraciones.
- Gestión de archivos y carpetas, Para organizar, almacenar y controlar la información digital para facilitar su búsqueda y recuperación 

### Personalización del Entorno

**Configuraciones aplicadas:** Se realizaron varias personalizaciones en el Visual Studio Code para mejorar la aparencia y la productividad del entorno. Se instaló el tema One Dark Pro, para asi obtener un fondo oscuro más comodo a la vista y el paquete de iconos Material Icon Theme, facilita la identificar los distintos tipos de archivos, también, se configuró la fuente Fira Code, con ligaduras activadas, mejorando la legibilidad del código, Además, se habilitó la opción de formateo automatico al guardar, el ajuste de línea y la detección de indentación automática para mantener el código ordenado. Se añadieron atajos de teclado útiles como Ctrl + / para comentar las lineas y Crtl + B para mostrar y ocultar la barra lateral

*Ejemplos de configuraciones útiles (elegir las que se consideren relevantes):*

**Temas e iconos:**
Ejemplos:
- Material Theme, One Dark Pro: ![Este es el paso anterior a instalar el fondo One Dark Pro](<Captura de pantalla 2025-11-06 191119.png>)
- File Icon Theme para mejor identificación de archivos

**Configuración de fuentes:**
Ejemplos:
- Fira Code, JetBrains Mono (con ligaduras)

**Atajos de teclado útiles:**
Ejemplos:
- Ctrl+/ para comentar/descomentar
- Ctrl+Shift+P para paleta de comandos
- Ctrl+` para terminal integrada
- Alt+↑/↓ para mover líneas: ![Aqui se muestra como hemos movido una linea con el atajo que pone antes](image.png)

**Configuración del editor:**
Ejemplos:
- Formateo automático al guardar
- Detección automática de indentación
- Word wrap para líneas largas

**Terminal integrada:**
Ejemplos:
- PowerShell como terminal predeterminado
- Configuración de perfil personalizado

> **Personaliza según tus necesidades**: Estas son sugerencias basadas en prácticas comunes. Experimenta y documenta las configuraciones que encuentres más útiles para tu flujo de trabajo.> 💼 **Manual de Incorporación**: Esta guía establece los estándares del equipo para configurar entornos de desarrollo en C#. Cualquier nuevo desarrollador debe poder seguir estas instrucciones para configurar su entorno de trabajo de manera consistente con el resto del equipo.

### SDK .NET

**Proceso de instalación:**
1. **Descarga e instalación:** Estando situados en la página de dotnet ![https://dotnet.microsoft.com/en-us/download](<Captura de pantalla 2025-11-06 222659-1.png>) instalamos el paquete de .net 9.0, unaa vez descargado nos salen varias pestañas. Damos a "abrir archivo" y nos sale otra pestaña ![esto es lo que sale cuando damos a "abrir archivo"](<Captura de pantalla 2025-11-06 223259-1.png>) le damos a instalar y una vez instalado nos sale otra pestaña![ esta es la pestaña que nos sale despues de instalarlo ](<Captura de pantalla 2025-11-06 223751-1.png>)
2. **Verificación:** ![Una vez instalado nos metemos en visual studio code y para comprobar que funciona vamos a la terminal y escribimos "dotnet" y nos sale esto](<Captura de pantalla 2025-11-06 234419-1.png>)

### Configuración para C#

**Extensiones esenciales:**
- **Soporte oficial para C#**: Extensión que proporciona IntelliSense, debugging y compilación


**Configuraciones específicas para C#:** 
Hay tres configuraciones:
    Formateo automático: Al guardar, el codigo se ordena y se corrige la indentacion
    IntelliSense: Sugiere codigo mientras escribes
    Compilador (dotnet build): Permite compilar desde la terminal

**Debugging básico:**
- Configuración de puntos de interrupción (breakpoints)
- Ejecutar y depurar
- Inspección de variables

> **Enfoque práctico**: Concentra tu documentación en las funcionalidades básicas que usarás día a día.

### Flujo de Trabajo con C#

**Creación de proyectos:**
A la hora de la creacion de proyectos para ejecutar el dotnet abrimos la terminal y ejecutamos poniendo dotnet y el nombre del proyecto y una linea mas abajo ponemos cd y el nombre del proyecto.

**Estructura de proyecto:**
```csharp
/// <summary>
/// Genera la secuencia de Collatz para un número inicial dado.
/// </summary>
/// <param name="initialNumber">Número inicial para generar la secuencia.</param>
void GenerateCollatzSequence(long initialNumber)
{
    while (initialNumber != 1)
    {
        if (initialNumber % 2 == 0)
            initialNumber = initialNumber / 2;
        else
            initialNumber = initialNumber * 3 + 1;

        Console.Write(initialNumber);
    }
}
```

**Compilación y ejecución:**
![El resultado de compilar y ejecutar](<Captura de pantalla 2025-11-07 112724-1.png>)

**Debugging:**
![Captura de lo que aparece cuando le das a "Run and](<Captura de pantalla 2025-11-07 112348-1.png>)

---

## Visual Studio - IDE Alternativo

### Instalación

**Proceso de instalación:**
- **Descarga:** ![Estando situados en la pagina oficial de visual studio](<Captura de pantalla 2025-11-07 171013.png>) ![Le damos a descargar, nos sale tres opciones y le damos  a desacargar download community ](<Captura de pantalla 2025-11-07 171023.png>) ![Una vez descargado le damos a abrir archivo y nos sale la pestaña que aparece a la izquierda de la captura](<Captura de pantalla 2025-11-07 171105.png>) 
- **Componentes necesarios:** ![Incluimos las herramientas que vamos a utilizar para .NET](<Captura de pantalla 2025-11-07 171515.png>)
- **Verificación:** [![Esto sirve para confirmar la version y los componentes instalados ](<Captura de pantalla 2025-11-07 174258.png>) ![Para comprobar que funciona ponemos un ejemplo de codigo](<Captura de pantalla 2025-11-07 175342.png>) ![Lo ejecutamos](<Captura de pantalla 2025-11-07 175750.png>)]

### Desarrollo con C#

**Creación de proyecto:**
[![Estando situados en la pagina principal de Visual Studio le damos a crear proyecto](<Captura de pantalla 2025-11-07 180642.png>) ![Seleccionamos la herramienta que vamos a utilizar](<Captura de pantalla 2025-11-07 180659.png>) ![Nombramos el proyecto y ponemos la ubicacion del archivo](<Captura de pantalla 2025-11-07 180858.png>) ![Elegimos la versión de .NET que queremos utilizar](<Captura de pantalla 2025-11-07 180911.png>) ![El archivo que nos genera Visual Studio automaticamente](<Captura de pantalla 2025-11-07 180930.png>)]

**Flujo de trabajo básico:**
- Compilación y ejecución: ![La captura de compilacion en la parte inferior](<Captura de pantalla 2025-11-07 181937.png>) ![La captura de depuracion en la parte inferior](<Captura de pantalla 2025-11-07 182018.png>)
- Uso de Solution Explorer: ![sale el panel derecho ](<Captura de pantalla 2025-11-07 182500.png>)
- Debugging básico: ![Empieza la depuracion del proyecto](<Captura de pantalla 2025-11-07 183239.png>) ![Acabamos la depuracion del proyecto](<Captura de pantalla 2025-11-07 183449.png>) 

---

## Configuración de Lenguaje Adicional

**Lenguaje seleccionado:** [Python] - **Justificación:** [Hemos seleccionado Python porque es un lenguaje fácil de aprender y versatil. Se utiliza en desarrollo web y ciencia de datos.]

### Instalación del Entorno

**Runtime/SDK:**
- **Descarga e instalación:** ![Estando situados en la pagina oficial de python descargamos la version de 64 bits para windows  ](<Captura de pantalla 2025-11-07 235744.png>) ![Una vez descargado le damos a "abrir archivo" y nos sale esta pestaña en la que seleccionamos la opcion "Add python.exe to PATH" y le damos a "Install now" ](<Captura de pantalla 2025-11-07 235800.png>) ![Una vez instalado nos sale esta pestaña](<Captura de pantalla 2025-11-08 000000.png>)
- **Verificación:** ![Para verificar que funciona correctamente ponemos Python en la terminal](<Captura de pantalla 2025-11-08 000710.png>) ![Hacemos un ejemplo con Python y lo ejecutamos para ver si funciona bien](<Captura de pantalla 2025-11-08 002021.png>) 

### Configuración en VS Code

**Extensiones por lenguaje:**
En nuestro caso hemos elegido python

*Para Java:*
- **Paquete completo de Java**: Incluye compilación, debugging y gestión de proyectos

*Para Python:*
- **Soporte oficial de Python**: 
Paso 1:Instalar extensiones de lenguaje:![Le damos a Ctrl+Shift+X para abrir el gestor de extensiones ](<Captura de pantalla 2025-11-08 134549.png>) ![Buscamos Python y Pylance y las instalamos](<Captura de pantalla 2025-11-08 130648.png>)

Paso 2:Seleccionamos el interprete: ![Abrimos un archivo .py](<Captura de pantalla 2025-11-08 135522.png>)![Le damos a Ctrl+Shift+P para abrir la paleta de comandos y seleccionamos la primera opcion en la que vamos a seleccionar el interprete que vamos a utilizar](<Captura de pantalla 2025-11-08 135609.png>) ![Seleccionamos el interprete de Python 3.13.9](<Captura de pantalla 2025-11-08 135717.png>)

*Para otros lenguajes:*
- Busca la extensión oficial del lenguaje que proporcione soporte completo

**Configuraciones específicas aplicadas:**
![Le damos a Ctrl+Shift+B para abrir la paleta de comandos y seleccionamos la primera opcion para abrir la configuracion de las herramientas de JSON](<Captura de pantalla 2025-11-08 131157.png>) ![Escribimos esto en dodne decimos las herramientas de JSON que vamos a utilizar y las configuramos ](<Captura de pantalla 2025-11-08 132752.png>)

### Proyecto de Ejemplo

**Código desarrollado:**
```[lenguaje]
// Código de ejemplo aquí
// Comentarios explicativos
```

**Proceso de ejecución:**
[Describir cómo ejecutar el código]

---

## Configuraciones Recomendadas

**Configuraciones generales:**
[![Cambiamos el tema ](<Captura de pantalla 2025-11-07 185637.png>) ![Le decimos que complie siempre que se pueda](<Captura de pantalla 2025-11-07 185907.png>)]

**Herramientas adicionales:**
ReSharper: Mejora la refactorización y la navegación
CodeMaid: limpio, tiene organización y formatea el código automaticamente
Github Copilot: Sugerencias inteligentes para escribir código más rápido


**Solución de problemas comunes:**
Si el proyecto no compila, revisa referencias en el Solution Explorer y vuelve a agregar las referencias.
Si no se encuentra el SDK instala el SDK correspondiente dessde la pagina oficial de dotnet.
Si el Visual Studio va lento desactiva las extenciones innecesarias y limpia el caché.



**Recursos útiles:**
- Enlace (https://dotnet.microsoft.com/es-es/download): Descargas SDKs y herramientas para .NET

- Documentación (https://learn.microsoft.com/es-es/visualstudio/?view=vs-2022): [Guia completa de todas las caracteristicas de Visual Studio] 

---
