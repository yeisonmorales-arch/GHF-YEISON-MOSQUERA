# PARQUEADERO AUTOMATICO DE 4 PUESTOS
El proyecto consiste en el diseño e implementación de un sistema automatizado de parqueadero con capacidad para cuatro vehículos, controlado mediante sensores y actuadores. Su objetivo principal es optimizar el proceso de entrada y salida de vehículos, reduciendo la intervención humana y mejorando la eficiencia en la gestión de espacios.

El sistema utiliza sensores infrarrojos para detectar la presencia de vehículos en cada puesto, y barreras automáticas controladas por un microcontrolador (como el Arduino) para permitir o restringir el acceso. Además, un display o interfaz visual muestra el estado de ocupación de cada puesto en tiempo real.

Este proyecto integra conceptos de electrónica, programación y control automático, aplicando principios de la ingeniería electrónica para desarrollar una solución funcional, escalable y de bajo costo para la gestión inteligente de parqueaderos.

# integrantes
- Yeison mosquera morales - 202570539
- David canal quintero - 202478461
- Ana Sofía Becerra Peláez - 202478498
- Maicol Steven Bermúdez Perea - 2478525

# rol de usuario
Como usuario del estacionamiento automatizado, mi rol principal consiste en interactuar con
el sistema desde el ingreso del vehículo hasta el retiro, garantizando que el proceso de
check in y check out se realice correctamente.
● Check in del vehículo: Mi responsabilidad es ingresar al sistema con el vehículo,
registrarlo mediante el proceso de check in y asegurar que quede asignado a una
zona de estacionamiento disponible.
● Supervisión de ocupación: Debo verificar en la plataforma o pantalla informativa
qué zonas de estacionamiento se encuentran ocupadas y cuáles están libres, con el
fin de conocer la disponibilidad en tiempo real.
● Check out del vehículo: Al momento de retirar el automóvil, debe realizar el
proceso de check out para que el sistema libere la zona ocupada y actualice el
estado de disponibilidad.
● Cumplimiento de normas: Me corresponde seguir las indicaciones de seguridad y
el flujo establecido por el sistema automatizado para evitar errores en la operación o
bloqueos en el proceso.
# OBJETIVOS DEL PROYECTO
Objetivo general:

Diseñar e implementar una planta de estacionamiento automatizado capacitada para
realizar el check in y check out de cada vehículo que entra en las instalaciones del recinto,
con el fin de gestionar de manera eficiente la disponibilidad de espacios y optimizar la
experiencia del usuario.

Objetivos específicos:

● Implementar un sistema de registro que permita identificar a cada vehículo en el
proceso de check in y check out de manera automatizada.
● Desarrollar una plataforma de visualización que muestre en tiempo real qué zonas
de estacionamiento se encuentran ocupadas y cuáles están libres.
● Integrar sensores, software y dispositivos de control que aseguren el correcto
funcionamiento del proceso de asignación y liberación de espacios.
● Evaluar el desempeño del sistema en condiciones reales de operación, identificando
fallas o incidencias para optimizar su eficiencia y confiabilidad.
● Promover el uso de tecnologías automatizadas en la gestión de estacionamientos,
resaltando su impacto en la modernización de infraestructuras urbanas y la
comodidad de los usuarios.

# Historias de usuario
1. Registro automático de ingreso de vehículo
ID: PU01
Nombre: Registro de vehículo entrante
Descripción: Como cliente, quiero que el sistema registre automáticamente mi vehículo al
ingresar al parqueadero, para asegurar que mi puesto se asigne correctamente y quede
registrado en la base de datos.
Valor de negocio: 10
Estimación de esfuerzo: 5
Prioridad: Must Have (M)
Criterios de aceptación:
El sistema recibe la señal del vehículo en tiempo real al entrar.
Se asigna automáticamente un puesto libre disponible y se registra en la base de datos.
Definition of Done:
El ingreso queda registrado correctamente y el puesto se marca como ocupado.
El cliente recibe confirmación de su puesto a través de la interfaz.

2. Visualización de estado de puestos
ID: PU02
Nombre: Estado de puestos en tiempo real
Descripción: Como cliente o administrador, quiero ver el estado actual de cada puesto
(ocupado/libre), para tomar decisiones rápidas y gestionar eficientemente el parqueadero.
Valor de negocio: 9
Estimación de esfuerzo: 3
Prioridad: Must Have (M)
Criterios de aceptación:
Cada puesto se muestra con su estado en la interfaz.
La información se actualiza automáticamente al ingresar o salir un vehículo.
Definition of Done:
Todos los puestos muestran correctamente su estado.
La actualización en tiempo real funciona sin retrasos.

3. Alerta de puesto ocupado
ID: PU03
Nombre: Notificación de ocupación
Descripción: Como cliente, quiero recibir una alerta si intento ocupar un puesto ya
ocupado, para evitar conflictos y asegurar la integridad de la asignación.
Valor de negocio: 8
Estimación de esfuerzo: 3
Prioridad: Should Have (S)
Criterios de aceptación:
El sistema bloquea la asignación de un puesto ocupado.
Se muestra un mensaje claro de “puesto ocupado” en la interfaz.
Definition of Done:
No se puede ocupar un puesto ya asignado.
La alerta se muestra correctamente y es comprensible.

4.  Liberación de puesto
ID: PU04
Nombre: Salida de vehículo
Descripción: Como cliente, quiero que al salir el sistema libere automáticamente mi puesto,
para que pueda ser utilizado por otro vehículo sin intervención manual.
Valor de negocio: 9
Estimación de esfuerzo: 4
Prioridad: Must Have (M)
Criterios de aceptación:
El servidor recibe la señal de salida del vehículo en tiempo real.
El puesto se marca como libre en la base de datos y en la interfaz.
Definition of Done:
El puesto queda libre correctamente al salir el vehículo.
Otros clientes pueden ocuparlo inmediatamente.

5. Asignación manual de puestos
ID: PU05
Nombre: Selección de puesto por el cliente
Descripción: Como cliente, quiero poder seleccionar manualmente un puesto libre, para
elegir la ubicación que prefiera dentro del parqueadero.
Valor de negocio: 7
Estimación de esfuerzo: 5
Prioridad: Could Have (C)
Criterios de aceptación:
Se muestran solo los puestos libres disponibles.
La selección se registra en la base de datos y se actualiza en la interfaz.
Definition of Done:
El puesto seleccionado se marca como ocupado.
No se puede seleccionar un puesto ocupado.

6. Registro de historial de ocupación
ID: PU06
Nombre: Historial de uso de puestos
Descripción: Como administrador, quiero poder consultar un historial de ocupación de los
puestos, para generar reportes y estadísticas de uso del parqueadero.
Valor de negocio: 6
Estimación de esfuerzo: 4
Prioridad: Should Have (S)
Criterios de aceptación:
Se registra la hora de ingreso y salida de cada vehículo.
Se pueden filtrar registros por puesto y fecha.
Definition of Done:
El historial se almacena correctamente en la base de datos.
La interfaz permite consultar y filtrar los datos.

7. Notificación de ingreso y salida
ID: PU07
Nombre: Confirmación al cliente
Descripción: Como cliente, quiero recibir confirmación al ingresar y al salir del
parqueadero, para tener seguridad de que mi información está registrada correctamente.
Valor de negocio: 7
Estimación de esfuerzo: 3
Prioridad: Should Have (S)
Criterios de aceptación:
Notificación al ingresar.
Notificación al salir.
Definition of Done:
El cliente recibe confirmación inmediata en la interfaz.
Las notificaciones coinciden con los eventos reales.

8. Bloqueo de ingreso si todos los puestos están ocupados
ID: PU08
Nombre: Bloqueo automático
Descripción: Como administrador, quiero que el sistema bloquee automáticamente el
ingreso de vehículos si todos los puestos están ocupados.
Valor de negocio: 8
Estimación de esfuerzo: 4
Prioridad: Must Have (M)
Criterios de aceptación:
Ningún ingreso adicional está permitido si todos los puestos están ocupados.
Se muestra el mensaje “Parqueadero lleno”.
Definition of Done:
Ingreso bloqueado correctamente.
El mensaje se muestra correctamente.

9. Visualización gráfica del parqueadero
ID: PU09
Nombre: Mapa interactivo de puestos
Descripción: Como cliente o administrador, quiero un mapa gráfico del parqueadero, para
identificar rápidamente los puestos libres y ocupados.
Valor de negocio: 7
Estimación de esfuerzo: 5
Prioridad: Should Have (S)
Criterios de aceptación:
Cada puesto se representa gráficamente en la interfaz.
La información se actualiza en tiempo real.
Definition of Done:
La interfaz muestra correctamente todos los puestos.
Los cambios de estado se reflejan instantáneamente.

10. Control de inconsistencias
ID: PU10
Nombre: Validación de estados de puestos
Descripción: Como administrador, quiero que el sistema valide la consistencia de los
estados de los puestos, para evitar conflictos de asignación.
Valor de negocio: 9
Estimación de esfuerzo: 5
Prioridad: Must Have (M)
Criterios de aceptación:
Sistema detecta y corrige inconsistencias de ocupación.
No se permite doble asignación de un mismo puesto.
Definition of Done:
Todos los puestos tienen estado consistente.
Conflictos de registro son prevenidos.

# Historias tecnicas
1. Integración de sensores de ingreso y salida
ID: TEC01
Descripción: Como desarrollador, quiero que el servidor reciba señales de ingreso y salida,
para actualizar el estado de los puestos automáticamente.
Valor de negocio: 9
Estimación de esfuerzo: 6
Prioridad: Must Have (M)
Criterios de aceptación:
Señales de ingreso y salida recibidas correctamente.
Puesto actualizado en la base de datos.
Definition of Done: Funcionamiento confiable y verificado.

2. Control de estados de puestos en tiempo real
ID: TEC02
Descripción: Como desarrollador, quiero que el servidor controle el estado ocupado/libre en
tiempo real, para reflejar correctamente la disponibilidad de cada puesto.
Valor de negocio: 8
Estimación de esfuerzo: 7
Prioridad: Must Have (M)
Criterios de aceptación:
Cada cambio de estado se registra correctamente.
Actualización en la interfaz sin retrasos.
Definition of Done: Sistema actualizado y funcional en tiempo real.

3. Sistema de notificaciones al cliente
ID: TEC03
Descripción: Como desarrollador, quiero que el sistema envíe notificaciones al cliente, para
confirmar ingreso, salida y alertas de puestos ocupados.
Valor de negocio: 7
Estimación de esfuerzo: 5
Prioridad: Should Have (S)
Criterios de aceptación:
Notificación enviada al ingresar y salir.
Alertas cuando un puesto está ocupado.
Definition of Done: Cliente recibe notificaciones correctamente

4. Registro de historial de ocupación
ID: TEC04
Descripción: Como desarrollador, quiero que el servidor registra un historial de uso de los
puestos, para generar reportes y estadísticas.
Valor de negocio: 6
Estimación de esfuerzo: 5
Prioridad: Should Have (S)
Criterios de aceptación:
Registro de hora de entrada y salida de cada vehículo.
Filtrado por puesto y fecha disponible en la interfaz.
Definition of Done: Historial generado y consultable sin errores.

# Casos de uso

Caso de Uso 1: Registrar entrada de vehículo
Actor principal: Conductor
Precondición: Debe haber al menos un puesto disponible.
Flujo principal:
- El conductor llega al parqueadero.
El sistema detecta la entrada del vehículo.
- El sistema descuenta un puesto disponible en el conteo.
- El sistema actualiza la pantalla con la nueva disponibilidad.
Flujo alterno:
- Si no hay puestos disponibles, el sistema muestra 'Parqueadero lleno' y no descuenta cupos.
Postcondición: El número de cupos libres disminuye en 1 (si había espacio).

Caso de Uso 2: Registrar salida de vehículo
Actor principal: Conductor
Precondición: Debe haber al menos un vehículo dentro.
Flujo principal:
- El conductor sale del parqueadero.
- El sistema detecta la salida.
- El sistema incrementa en 1 el número de cupos libres.
- El sistema actualiza la pantalla con la nueva disponibilidad.
Flujo alterno:
- Si no había vehículos, no se realiza el incremento.
Postcondición: El número de cupos libres aumenta en 1 (si había vehículos).

Caso de Uso 3: Consultar disponibilidad
Actor principal: Conductor
Precondición: El sistema debe estar encendido.
Flujo principal:
- El conductor se acerca a la pantalla del sistema.
- El sistema muestra la cantidad de puestos libres.
Flujo alterno:
- Si el sistema falla, se muestra un mensaje de error.
Postcondición: El conductor conoce cuántos cupos hay disponibles.

Caso de Uso 4: Mostrar cupos libres
Actor principal: Sistema
Precondición: El parqueadero no debe estar lleno.
Flujo principal:
- El sistema registra cada entrada o salida de vehículo.
- El sistema actualiza la pantalla mostrando la cantidad de puestos libres.
Flujo alterno:
- Si todos los puestos están ocupados, se activa el caso 'Mostrar parqueadero lleno'.
Powered by
CS CamScanner
Postcondición: La pantalla refleja el número correcto de cupos libres.

Caso de Uso 5: Mostrar parqueadero lleno
Actor principal: Sistema
Precondición: Todos los puestos deben estar ocupados.
Flujo principal:
- El sistema detecta que el número de puestos libres es cero.
- El sistema muestra en la pantalla el aviso 'Parqueadero lleno'.
Flujo alterno:
Cuando un vehículo salga, se vuelve al caso 'Mostrar cupos libres'.
Postcondición: El usuario es informado de que no hay cupos.

Caso de Uso 6: Reiniciar sistema
Actor principal: Administrador
Precondición: El sistema debe estar encendido.
Flujo principal:
- El administrador selecciona la opción de reinicio.
- El sistema detiene las operaciones actuales.
- El sistema inicializa los contadores a cero.
- El sistema queda listo para registrar nuevas entradas y salidas.
Flujo alterno:
- Si el reinicio falla, el sistema muestra un mensaje de error.
Postcondición: El sistema queda restablecido y el conteo reiniciado.

# diagrama de clases
![Imagen de WhatsApp 2025-10-23 a las 20 58 20_df67ff07](https://github.com/user-attachments/assets/e583d236-991e-4800-85a7-e49d5f860ab5)

# diagrama de estados
![Imagen de WhatsApp 2025-10-31 a las 09 37 18_68614ce3](https://github.com/user-attachments/assets/9be8b18b-a56d-42b1-93c5-354a39e987dc)

# reunion por meet (12 de noviembre del 2025) 
![Imagen de WhatsApp 2025-11-12 a las 14 03 03_aa85c3f6](https://github.com/user-attachments/assets/7c40a5cc-d931-453e-a774-a8a5902f4f78)

![Imagen de WhatsApp 2025-11-12 a las 14 03 48_29fbd546](https://github.com/user-attachments/assets/8597e62f-4765-40b4-b3f7-e945d7a4da33)












