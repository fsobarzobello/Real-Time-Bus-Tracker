# Real-Time-Bus-Tracker

Este proyecto muestra cómo crear un marcador animado en un mapa de Mapbox para resaltar las rutas del autobús entre MIT y Harvard usando los datos del MBTA.

## Instrucciones de Configuración

### Prerrequisitos

- Una cuenta de Mapbox con un token de acceso.

### Archivos en el Proyecto

- `index.html`: El archivo HTML principal que incluye el mapa de Mapbox y un botón para iniciar la animación.
- `styles.css`: Contiene estilos básicos para el mapa y la superposición.
- `mapanimation.js`: El archivo JavaScript que inicializa el mapa, agrega el marcador y define la lógica de animación.

### Instrucciones

1. **Crear una Cuenta en Mapbox y Obtener el Token de Acceso**:
   - Ve a [Mapbox](https://www.mapbox.com/) y crea una cuenta.
   - Genera un token de acceso desde tu cuenta.

2. **Crear el Archivo `token.js`**:
   - En la misma carpeta del proyecto, crea un archivo llamado `token.js`.
   - Añade el siguiente contenido al archivo, reemplazando `'TU_TOKEN_DE_ACCESO'` con tu propio token de acceso de Mapbox:
     ```javascript
     const token = 'TU_TOKEN_DE_ACCESO';
     ```

3. **Ejecutar el Proyecto**:
   - Abre `index.html` en tu navegador.
   - Haz clic en el botón "Show stops between MIT and Harvard" para iniciar la animación del marcador en el mapa.

### Descripción del Código

- **`mapanimation.js`**:
  - Define los paraderos de autobús entre MIT y Harvard en un array.
  - Inicializa el mapa de Mapbox con el token de acceso.
  - Agrega un marcador en el primer paradero de autobús.
  - Define la función `move()` que se llama cuando se selecciona el botón, moviendo el marcador a cada paradero de autobús cada 1000 ms.

## Roadmap de Futuras Mejoras

En futuras mejoras, se puede mejorar en lo siguiente:
- Agregar una interfaz de usuario para seleccionar diferentes autobuses y sus rutas.
- Agregar opciones de personalización para los marcadores y distintos layout para el mapa como vista satelital o solo las calles.
- Mostrar información en tiempo real de la posición del autobús para que el usuario sepa en cuanto puede llegar el bus.

### License

Este proyecto está bajo la licencia MIT. Consulte el archivo LICENSE para obtener más detalles.
