Resumen del Sistema de Registro de Usuarios

Descripción del caso

El sistema de registro de usuarios es una aplicación sencilla de software diseñada para el manejo de cuentas de usuario. Su propósito principal es gestionar la identidad básica de los usuarios, con un enfoque en mantener la información personal actualizada

Objetivos

El propósito del sistema es gestionar la creación, autenticación y administración de cuentas de usuario dentro de una aplicación, con el objetivo de garantizar la seguridad del acceso, proteger la información personal de los usuarios y permitir una experiencia personalizada según los privilegios y funciones asignadas a cada cuenta.

REQUERIMIENTOS

Requerimientos Funcionales (RF):

RF1 Registro de Nuevo Usuario: El sistema debe permitir al usuario ingresar su nombre, correo electrónico y una contraseña segura para crear una cuenta.
RF2 Inicio de Sesión: El sistema debe autenticar al usuario utilizando su correo electrónico y contraseña.
RF3 Modificación de inicio de sesión: El usuario debe de actualizar su correo electrónico y contraseña una vez que ha iniciado sesión.
RF4 Validación de Credenciales: El sistema debe verificar que el correo electrónico no exista previamente durante el registro.
RF5 Recuperación de Contraseña: El sistema debe permitir al usuario restablecer su contraseña a través de un mecanismo seguro (ej. envío de enlace por correo).
Requerimientos No Funcionales (RNF):

RNF1 Seguridad: El sistema debe almacenar las contraseñas de los usuarios utilizando un algoritmo de cifrado robusto.
RNF2 Rendimiento: El tiempo de respuesta para el proceso de inicio de sesión no debe exceder los 2 segundos.
RNF3 Usabilidad: La interfaz de usuario para el registro y la modificación del perfil debe ser intuitiva y fácil de usar.
Casos de prueba

Prueba Unitario (RF1): La prueba de Registro de Nuevo Usuario con datos de entrada (Usuario: Juan Pérez, Correo: juan@mail.com, Contraseña: Segura123) tuvo como Resultado Obtenido: Usuario creado y autenticado correctamente (exitoso).
Prueba Unitario (RF2): La prueba de Inicio de Sesión con Contraseña: Incorrecta tuvo como Resultado Obtenido: Mensaje de error correcto ("Credenciales inválidas") (Error detectado).
Prueba Unitario (RF4): La prueba de Validación de Credenciales con un Intento de registro con correo que ya existe dio como Resultado Obtenido: Solicitud rechazada correctamente (exitoso), mostrando el mensaje: "El correo ya está registrado".
Prueba Validación (RNF2): La Ejecución de la prueba de Rendimiento (Modificación de perfil) tenía como resultado esperado que el proceso de actualización debe tomar menos de 2 segundos. El Resultado Obtenido fue 1.5 segundos (Criterio cumplido) (exitoso).
Prueba Validación (RF3): La prueba de Modificación de Perfil (Usuario cambia su nombre de "Juan Pérez" a "Juan A. Pérez") dio como Resultado Obtenido: Perfil actualizado y persistente (exitoso).
Tipo de mantenimiento propuesto

Mantenimientos aplicables al Sistema de Registro de Usuarios Tipo: Mantenimiento Perfectivo

Acción: Implementar mejoras continuas orientadas a optimizar el rendimiento, la seguridad y la usabilidad del sistema, incluyendo la incorporación de nuevas funcionalidades como la verificación de correo electrónico, la actualización de librerías y protocolos, y la optimización de consultas en la base de datos.

Justificación:El mantenimiento perfectivo se enfoca en mejorar y evolucionar el software, aun cuando no existan fallas, con el fin de adaptarlo a nuevas necesidades, entornos tecnológicos o requerimientos de desempeño. Este tipo de mantenimiento asegura que el sistema siga siendo eficiente, vigente y escalable a futuro, alineándose con la teoría que establece que el mantenimiento perfectivo busca optimizar la calidad del producto mediante ajustes y ampliaciones progresivas.

Tipo: Mantenimiento Correctivo Acción: Corregir errores o inconsistencias presentes en los procesos de validación, manejo de la autenticación, o cualquier falla detectada durante la operación del sistema.

Justificación: El mantenimiento correctivo se centra en resolver fallos que afectan el funcionamiento normal del sistema y que pueden comprometer la experiencia del usuario o la integridad de los datos. Este tipo de mantenimiento es complementario al perfectivo, ya que ninguna mejora garantiza la calidad total del software si no se atienden primero los errores que puedan interferir con su operación. Su fundamento teórico establece que este mantenimiento restaura el comportamiento esperado del sistema ante desviaciones o defectos detectados.

Reflexión sobre el control de versiones

El control de versiones se vuelve una herramienta clave en el desarrollo de un sistema de registro de usuarios, porque no solo permite llevar un historial claro y ordenado de cada cambio realizado, sino que también garantiza la integridad y calidad del software a medida que evoluciona. En proyectos donde se manejan datos sensibles y funcionalidades críticas como la creación, autenticación y actualización de cuentas, contar con un sistema de versiones evita errores, facilita revertir fallas y ayuda a que todo el equipo trabaje sincronizado sin pisarse el código. Además, promueve una cultura de organización y responsabilidad, ya que cada modificación queda documentada, lo que mejora la trazabilidad de decisiones técnicas. En definitiva, el control de versiones no es solo una herramienta técnica, sino una buena práctica que impulsa la confianza, la seguridad y la mantenibilidad de cualquier sistema que maneje información de usuarios
