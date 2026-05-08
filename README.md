# PROVISER Asset Tracking – Sistema de control y trazabilidad de inventarios

<img width="1600" height="803" alt="6" src="https://github.com/user-attachments/assets/a79f8f93-ada6-44b4-aac7-2ab697a3c4b3" />
*Vista principal con los módulos disponibles para el personal de PROVISER Ltda.*

## Descripción general

**PROVISER Asset Tracking** es un prototipo funcional de sistema digital desarrollado sobre la plataforma **AppSheet** (no-code) para la empresa PROVISER Ltda., dedicada a servicios de seguridad física en Cali, Colombia. El sistema resuelve las limitaciones del proceso actual basado en hojas de cálculo Excel, ofreciendo:

- Registro automatizado de entradas y salidas de inventario mediante códigos QR.
- Geolocalización y firma digital para validar entregas de equipos en campo.
- Módulos de reportes y auditoría en tiempo real.
- Evaluación de viabilidad de integración con tecnología RFID como mejora futura.

El proyecto fue desarrollado como trabajo de grado de Ingeniería de Sistemas (UNAD) y actualmente se encuentra en fase de implementación piloto.

## Módulos principales del prototipo

### 1. Gestión de clientes

<img width="1600" height="799" alt="5" src="https://github.com/user-attachments/assets/68d7ece3-a252-4b0f-985e-01a5064a8136" />
*Vista de la estructura de datos del módulo Clientes, con campos como NIT, dirección, representante y relaciones con contratos, salidas e instalaciones.*

El sistema permite administrar la base de datos de clientes, incluyendo información de contacto, ubicación y referencias cruzadas a todos los movimientos asociados (contratos, salidas de equipos, instalaciones, mantenimientos).

### 2. Módulo de contratos

<img width="1600" height="371" alt="2" src="https://github.com/user-attachments/assets/7a6a3ba2-697e-4e64-a131-6ee314e49c94" />
*Vista superior del módulo Contratos, con acceso para crear nuevos contratos, listar existentes y gestionar servicios asociados.*

Cada contrato se vincula directamente con los equipos asignados y las salidas registradas, permitiendo un seguimiento integral por cliente.

### 3. Registro de salida de equipos (con QR y geolocalización)

<img width="728" height="637" alt="3" src="https://github.com/user-attachments/assets/a0966a60-c966-4562-9202-d9cd91293908" />
*Formulario de salida con campos para contrato, ID del equipo (escaneo QR), fecha automática, persona que recibe, identificación y foto de evidencia.*

Esta es la pantalla central del sistema. Al escanear un código QR fijado en cada activo, el formulario se llena automáticamente y se captura:
- Fecha y hora.
- Geolocalización del punto de entrega (mediante GPS del dispositivo móvil).
- Firma digital del receptor (integrada en versiones posteriores, no visible en esta captura).
- Fotografía de evidencia.

### 4. Navegación y menú de accesos rápidos

<img width="1600" height="794" alt="4" src="https://github.com/user-attachments/assets/af54d2da-66c6-4f54-bb98-be58ce846b3e" />
*Estructura del menú en el editor de AppSheet, mostrando las opciones de navegación: Inicio, Almacén, Clientes, Contratos, Historial de Importancia, Salida Equipos, Eliminar salidas, etc.*

El prototipo incluye un panel lateral (sidebar) que agrupa todas las operaciones del almacén, así como reportes específicos y acciones de administración.

### 5. Dashboard de inicio (acceso a todas las funciones)

<img width="1600" height="803" alt="6" src="https://github.com/user-attachments/assets/bbc171de-643b-45c3-985c-55f369a11cd5" />
*Vista de inicio del aplicativo que lista los accesos directos a: Mapas, Instalación de dispositivos, Clientes, Usuarios, Inventario de dispositivos, Histórico de mantenimientos, Salida de equipos, Inventario de armamento, Salida de armas, Instalación de armas, Módulo Contratos, Módulo Importados y eliminaciones.*

Desde aquí, los operarios de almacén y técnicos de campo pueden ejecutar cualquier transacción sin necesidad de recurrir al Excel.

## Tecnologías utilizadas

- **Plataforma**: AppSheet (Google)
- **Base de datos backend**: Google Sheets (con relaciones entre tablas)
- **Identificación**: Códigos QR impresos en etiquetas adheridas a cada equipo
- **Localización**: GPS nativo de dispositivos móviles (Android/iOS)
- **Firma digital**: Captura mediante touchpad del móvil (implementado en el sistema aunque no se ve en las capturas)
- **Futura mejora**: Evaluación de lectores RFID UHF para alertas de salidas no autorizadas

## Estado del proyecto

✅ Fase de diagnóstico completada  
✅ Diseño de la solución en AppSheet finalizado  
✅ Prototipo funcional desplegado en entorno de pruebas  
🔄 Implementación piloto con personal de almacén de PROVISER Ltda. (en curso)  
⏳ Evaluación de resultados y ajustes  
⏳ Documentación técnica de viabilidad RFID

## Capturas adicionales (estructura de datos)

<img width="1600" height="799" alt="5" src="https://github.com/user-attachments/assets/3c157410-025c-4c47-9449-303979ec387c" />
*Se muestra la definición de la tabla "Clientes" dentro de AppSheet, con sus columnas, tipos de datos, y referencias a tablas relacionadas (Contratos, Salidas, Instalaciones, etc.). Esta estructura garantiza la trazabilidad completa.*

## Cómo contribuir o probar

Este repositorio contiene el prototipo del sistema PROVISER Asset Tracking. Para acceder al aplicativo funcional se requiere autorización de PROVISER Ltda. Sin embargo, el diseño y la documentación pueden ser reutilizados bajo licencia académica.

Si deseas conocer más detalles del proyecto (metodología, objetivos, marco teórico, referencias), consulta el documento `Proyecto_Grado_PROVISER.pdf` incluido en este repositorio.

---

**Autores**  
Efren Ordoñez Joyas – eordonezj@unadvirtual.edu.co  
John Harold Aguirre Martinez – jhaguirrem@unadvirtual.edu.co  

**Tutor**  
Ruben Dario Ordoñez  

**Institución**  
Universidad Nacional Abierta y a Distancia – UNAD  
Programa de Ingeniería de Sistemas  
Cali, Colombia – 2026
