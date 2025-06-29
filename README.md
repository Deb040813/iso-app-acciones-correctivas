# iso-app-acciones-correctivas
Aplicación para subir acciones correctivas de ISO 9001:2015
# ISO App Robusta - Gestión de Acciones Correctivas ISO 9001:2015

Este proyecto es una aplicación web de una sola página (SPA) diseñada para dar seguimiento a las acciones correctivas en una organización que cumple con la norma ISO 9001:2015.

## Características principales

### 👥 Gestión de usuarios
- Inicio de sesión por nombre de usuario.
- Panel individual de acciones correctivas asignadas.

### 👩‍💼 Panel para Sistema de Gestión
- Solo el usuario `sistema.calidad` puede agregar nuevas acciones correctivas.
- Se puede asignar cada acción a un responsable específico.

### 📁 Subida de evidencias
- Cada usuario puede subir evidencia (simulada) por cada acción.
- Muestra el avance individual en formato de barra y gráfico.

### 📊 Dashboard personal
- Visualización de las acciones asignadas al usuario.
- Gráfico de barras en tiempo real con evidencias completadas vs requeridas.

### 🧮 Dashboard global (solo para sistema.calidad)
- Muestra un resumen tabular del avance de todos los usuarios.

## Requisitos
- Navegador web moderno (Google Chrome, Firefox, Edge).
- Editor como Visual Studio Code (opcional para personalización).

## Cómo usar
1. Abre el archivo HTML en tu navegador.
2. Inicia sesión con tu nombre.
   - Si eres del equipo de gestión, usa: `sistema.calidad`
3. Como `sistema.calidad` puedes:
   - Agregar nuevas acciones (ID, nombre, evidencias requeridas y responsable).
   - Visualizar el dashboard global.
4. Como usuario responsable:
   - Verás solo tus acciones.
   - Podrás subir evidencias y ver tu progreso.

## Estructura del código
- HTML con Bootstrap para diseño.
- JavaScript nativo con Chart.js para gráficos.
- `axios` preparado para futuras integraciones con webhooks o base de datos.

## Siguientes pasos sugeridos
- Conexión con Google Sheets vía Make o Zapier.
- Almacenamiento real de archivos (Drive o base de datos).
- Exportación a Excel/CSV del dashboard global.
- Agregar login con autenticación real.

---
