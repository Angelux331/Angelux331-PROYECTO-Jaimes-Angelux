# Panel de Indicadores

## Descripción

Este proyecto es un **panel de indicadores** que permite gestionar y visualizar métricas clave de un equipo o proyecto. La aplicación está diseñada con **HTML, CSS y un enfoque de maquetación accesible**, mostrando los datos en un formato de **tabla interactiva con progreso visual**.

El panel incluye funcionalidades para:

- Visualizar indicadores existentes.  
- Añadir nuevos indicadores mediante formularios.  
- Eliminar indicadores seleccionados.  
- Reportar problemas, bugs o sugerencias del sistema.  

El diseño es **responsivo y accesible**, con etiquetas ARIA y roles para mejorar la navegación de usuarios con lectores de pantalla.

---

## Tecnologías utilizadas

- **HTML5** – Estructura semántica de la página.  
- **CSS3** – Estilos, layout con `flex` y `grid`, y barra de progreso animada usando variables CSS (`--p`).  
- **Maquetación responsiva** – Uso de `max-width`, `flex-direction`, `text-align` y `margin auto` para centrar contenido.  

> Nota: Actualmente el proyecto funciona como maqueta; no incluye backend ni base de datos, por lo que los botones de “Añadir”, “Eliminar” o “Reportar” no envían información a un servidor real.  

---

## Estructura del proyecto

/
├─ index.html # Página principal del panel
├─ css/
│ └─ styles.css # Estilos globales y específicos
├─ assets/ # Imágenes, íconos y logos
└─ pages/
├─ fqa.html # Sección de ayuda
└─ profile.html # Perfil de usuario


---

## Funcionalidades principales

### Vista principal
- Muestra todos los indicadores en un **grid con columnas**:  
  Indicador | Descripción | Categoría | Fechas | Fórmula | Frecuencia | Cumplimiento | Área | Acciones  
- Cada fila tiene un **indicador de progreso circular** para representar el cumplimiento.  
- Botones de acción rápida: **Añadir**, **Refrescar**, **Eliminar**.  

### Añadir indicador
- Formulario para registrar un nuevo indicador:  
  - Nombre  
  - Descripción  
  - Categoría y Área  
  - Fecha de inicio y terminación  
  - Fórmula y frecuencia  
  - Porcentaje inicial de cumplimiento  
- Botón para guardar o cancelar la acción.

### Eliminar indicadores
- Permite **seleccionar y eliminar indicadores** del panel (simulado en la maqueta).  
- Muestra una advertencia de que la acción es **permanente**.

### Reportar un problema
- Formulario para reportar errores o sugerencias:  
  - Tipo de reporte  
  - Título y descripción  
  - Pasos para reproducir el error  
  - Prioridad y navegador utilizado  
  - Email del usuario  
- Mensaje de confirmación indicando que el reporte será revisado.

---

## Uso

1. clonar el respositorio con (git clone https://github.com/Angelux331/Angelux331-PROYECTO-Jaimes-Angelux)
2. Abrir el archivo `index.html` en un navegador moderno (Chrome, Firefox, Edge).  
3. Navegar entre las secciones usando la **barra de navegación superior**.  
4. Interactuar con los indicadores, formularios y botones según la maqueta.  

> Tip: Los inputs tipo `radio` se usan para cambiar de vista entre **principal, añadir, eliminar y reportar**.

---

## Personalización

- **Barra de progreso**: Modifica el porcentaje cambiando la variable CSS `--p` en cada `div.progress-ring`.  
- **Colores**: Se pueden cambiar según nivel de cumplimiento (`green`, `orange`, `red`).  
- **Estilos**: Se pueden personalizar los botones, tipografía y layout en `css/styles.css`.  

---

## Futuras mejoras

- Conectar a un **backend** para almacenar los indicadores en base de datos.  
- Hacer que los botones **Añadir, Eliminar y Reportar** funcionen de forma real.  
- Agregar **filtrado y búsqueda** de indicadores.  
- Implementar **notificaciones dinámicas** en tiempo real.  

---

## Figma
[Figma](https://www.figma.com/design/2Zi2CH2EANIrKoUyRziCj7/Untitled?node-id=0-1&t=18tzOTYrac8b5Lwp-1)

## Licencia

Este proyecto es **libre para uso educativo y de maqueta**. No se proporciona licencia comercial.
