# CarClicker

CarClicker es una aplicacion web simple que implementa el patron de arquitectura MVC (Model-View-Controller) utilizando solo JavaScript vanilla. El proyecto esta diseñado como practica para comprender los conceptos fundamentales del desarrollo web con JavaScript.

## Descripcion del Proyecto

CarClicker es una aplicacion de votacion interactiva que permite a los usuarios seleccionar diferentes tipos de coches muscle de una lista y aumentar su contador de clics haciendo clic en la imagen del coche seleccionado.

La aplicacion sigue el patron MVC:
- **Model (Modelo)**: Almacena los datos de los coches (nombre, imagen y contador de clics)
- **View (Vista)**: Maneja la presentacion grafica y la interaccion con el usuario
- **Controller (Controlador)**: Coordina el flujo de datos entre el modelo y la vista

## Caracteristicas

- Lista de coches muscle clasicos
- Seleccion de coche haciendo clic en la lista
- Contador de clics que aumenta al hacer clic en la imagen
- Interfaz responsiva gracias a Bootstrap
- Sin dependencias locales - todo se carga desde CDN

## Descripcion de Componentes

### Model (Capa de Datos)
- **Tecnologia**: JavaScript ES6+ (vanilla)
- **Estructura**: Objeto `model` con dos propiedades:
  - `currentCar`: Referencia al objeto del coche seleccionado
  - `cars`: Array de objetos que almacena cada coche con sus propiedades
- **Almacenamiento**: En memoria (no persistente)

### View (Capa de Presentacion)
- **Tecnologias**:
  - HTML5 (estructura del DOM)
  - Bootstrap 4.4.1 (CSS desde CDN)
  - jQuery 3.4.1 (manipulacion del DOM desde CDN)
  - Popper.js 1.16.0 (dependencia de Bootstrap, desde CDN)
  - Bootstrap JS 4.4.1 (componentes interactivos desde CDN)
- **Componentes**:
  - `carListView`: Renderiza la lista de coches en el panel lateral
  - `carView`: Renderiza la imagen, nombre y contador del coche seleccionado

### Controller (Capa de Control)
- **Tecnologia**: JavaScript ES6+ (vanilla)
- **Funcion**: Coordina las interacciones entre Model y View:
  - Inicializa la aplicacion estableciendo el estado inicial
  - Expone metodos publicos para acceder y modificar el modelo
  - Detecta eventos de clic en la vista y actualiza el modelo
  - Invoca el metodo `render()` de la vista despues de cada cambio

## Coches Disponibles

- Coupe Maserati
- Camaro SS 1LE
- Dodger Charger 1970
- Ford Mustang 1966
- 190 SL Roadster 1962

## Requisitos

- Navegador web moderno (Chrome, Firefox, Safari, Edge)
- Conexion a internet (necesario para cargar Bootstrap y jQuery desde CDN)

## Instrucciones de Ejecucion

### Opcion 1: Abrir directamente en el navegador

1. Navega al directorio donde clonaste o descomprimiste el proyecto
2. Haz doble clic en el archivo `index.html`
3. La aplicacion se abrira en tu navegador predeterminado

### Opcion 2: Usar un servidor local

Si deseas ejecutar la aplicacion desde un servidor local (recomendado para mejor experiencia de desarrollo):

## Estructura del Proyecto

```
CarClicker/
├── index.html          # Archivo principal HTML
├── js/
│   └── app.js         # Logica JavaScript (MVC)
├── img/               # Imagenes de los coches
│   ├── black-convertible-coupe.jpg
│   ├── chevrolet-camaro.jpg
│   ├── dodge-charger.jpg
│   ├── ford-mustang.jpg
│   └── mercedes-benz.jpg
└── README.md          # Este archivo
```

## Uso de la Aplicacion

1. Al abrir la aplicacion, veras una lista de coches a la izquierda
2. Haz clic en cualquier coche de la lista para seleccionarlo
3. La imagen del coche seleccionado aparecera en el panel derecho
4. Haz clic en la imagen del coche para incrementar su contador de clics
5. El numero de clics se actualizara automaticamente

## Tecnologias Utilizadas

- HTML5
- CSS3 (a traves de Bootstrap 4.4.1)
- JavaScript ES6+ (vanilla, sin frameworks)
- Bootstrap 4.4.1 (desde CDN)
- jQuery 3.4.1 (desde CDN)

## Licencia

Este proyecto libre y es de uso educativo.
