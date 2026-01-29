AppBiblioteca: Sistema de Gestión con Patrón MVC

Proyecto desarrollado para la Tarea Online 5 del módulo de Programación (Grado Superior DAM). Esta aplicación implementa un sistema robusto de gestión de bibliotecas utilizando Java, el sistema de construcción Gradle y una arquitectura basada en el patrón Modelo-Vista-Controlador (MVC).
Características Principales

    Arquitectura MVC: Separación estricta entre la lógica de negocio, la interfaz de usuario (consola) y el control de flujo.

    Validación Defensiva: Implementación de expresiones regulares (Regex) para validar DNI, ISBN y códigos postales en tiempo real.

    Gestión de Inventario Real: Control estricto de unidades disponibles. El sistema impide préstamos si no hay existencias y actualiza el stock automáticamente al devolver ejemplares.

    Integridad de Datos: Uso de constructores copia en todas las entidades del dominio para garantizar la inmutabilidad y seguridad de la información.

    Entrada de Datos Robusta: Integración de la librería Entrada para una gestión de errores de teclado eficiente.

Tecnologías Utilizadas

    Lenguaje: Java 17+

    Gestor de Dependencias: Gradle

    IDE: IntelliJ IDEA

    Librerías: org.iesalandalus.programacion.utilidades.Entrada

Estructura del Proyecto

El código se organiza siguiendo la jerarquía de paquetes definida en el diagrama de clases oficial:

    biblioteca.controlador: Intermediario entre vista y modelo.

    biblioteca.modelo: Gestión de la lógica de datos.

        .dominio: Clases básicas (Libro, Usuario, Prestamo, etc.).

        .negocio: Colecciones y reglas de negocio (Libros, Usuarios, Prestamos).

    biblioteca.vista: Interfaz de consola y gestión de menús.

💻 Instalación y Ejecución

    Clonar el repositorio:

    git clone https://github.com/IsakAndueza/biblioteca_mvc.git

    Importar en IntelliJ: Abrir el archivo build.gradle como proyecto.

    Ejecución: Ejecutar la clase AppBiblioteca ubicada en el paquete raíz biblioteca.
