 Llanquihue Tour Management System 🌲🚌

1. Descripción del Proyecto
Este proyecto es un prototipo de software desarrollado para la agencia de turismo Llanquihue Tour, ubicada en la región de Los Lagos. El sistema tiene como propósito resolver la desorganización de datos y la falta de trazabilidad en los registros de la empresa. 

Mediante el uso de Programación Orientada a Objetos (POO) en Java, el software unifica la información de clientes, guías y operadores, eliminando la duplicidad de datos y permitiendo una clasificación clara de roles a través de los pilares de herencia y composición.

 2. Propósito y Problemática Abordada
El sistema busca mitigar los siguientes puntos críticos:
- Centralización de datos: Evita que la información esté distribuida en múltiples archivos sin estructura.
- Diferenciación de roles: Permite distinguir entre una persona general y un empleado con funciones específicas.
- Reutilización de código: Utiliza una clase base para atributos comunes, reduciendo errores y retrabajos en el desarrollo.

 3. Estructura de Paquetes y Clases
El proyecto sigue una arquitectura modular dividida en dos paquetes principales:

📦 Paquete: `model` (Lógica del Dominio)
Contiene las clases que representan las entidades del negocio:
- `Direccion`: Clase componente que almacena calle, número y ciudad. Se integra en otras clases mediante composición.
- `Persona`: Clase base general que contiene atributos comunes como RUT, nombre y teléfono.
- `Empleado`: Clase especializada que hereda de `Persona`. Añade atributos de contrato como rol (Guía/Operador) y sueldo base.

📦 Paquete: `app` (Ejecución)
- `Main`: Clase principal que orquesta la creación de objetos, realiza las pruebas de instanciación y despliega la información formateada en la consola del sistema.


4. Instrucciones de Compilación y Ejecución

Para ejecutar este prototipo en tu entorno local siguiendo los estándares de IntelliJ IDEA, sigue estos pasos:

 Prerrequisitos
- Tener instalado el JDK 11 o superior.
- Utilizar IntelliJ IDEA (recomendado) o cualquier IDE compatible con Java.

### Pasos para Ejecutar
1. Importar el Proyecto:
   - Abre IntelliJ IDEA y selecciona `File > Open`.
   - Navega hasta la carpeta raíz del proyecto y selecciónala.
2. Compilar:
   - Haz clic en el menú superior `Build > Build Project`.
3. Ejecutar la Clase Main:
   - En el explorador de proyectos (izquierda), despliega la ruta: `src/app/Main.java`.
   - Haz clic derecho sobre el archivo `Main.java` y selecciona la opción Run 'Main.main()'.
4. Verificar Salida:
   - Los resultados de la trazabilidad de objetos se mostrarán automáticamente en la pestaña Run de la parte inferior del IDE.



