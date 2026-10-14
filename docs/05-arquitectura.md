# Arquitectura de la información — El Sauce Huevitos

> Guía: [Arquitectura de la información](../evaluacion/guias/fase-1-requerimientos/05-arquitectura.md)

## Mapa de sitio

```text
Inicio (Landing)
├── Buscar
│   ├── Buscar productos
│   └── Buscar artículos del blog
│
├── Tienda
│   ├── Huevos
│   ├── Frutos secos
│   ├── Mermeladas y manjar artesanal
│   ├── Otros productos
│   ├── Filtros por categoría
│   ├── Detalle del producto
│   ├── Carrito de compras
│   └── Confirmación del pedido
│
├── Blog
│   ├── Alimentación
│   ├── Consejos y recomendaciones
│   ├── Recetas
│   ├── Artículos por categoría
│   └── Detalle del artículo
│
├── Sobre nosotros
│   ├── Historia del emprendimiento
│   └── Propuesta de valor
│
├── Despachos
│   ├── Zonas de entrega
│   ├── Costos de despacho
│   └── Condiciones de entrega
│
├── Contacto
│   ├── WhatsApp
│   ├── Instagram
│   └── Ubicación del emprendimiento
│
├── Preguntas frecuentes
│
├── Suscripción a novedades
│
├── Políticas de la empresa
│   ├── Política de privacidad
│   ├── Términos y condiciones
│   ├── Política de cambios y devoluciones
│   └── Política de despacho
│
├── Página 404 (Página no encontrada)
│
└── Pie de página (Footer)
    ├── Datos de contacto
    ├── Redes sociales
    ├── Enlaces de navegación
    └── Políticas de la empresa
```

## User flows

> Guía: [User flow](../evaluacion/guias/fase-1-requerimientos/06-user-flow.md)

### Flujo 1: compra de productos

```text
Inicio
  ↓
Tienda
  ↓
Buscar producto o elegir categoría
  ↓
Ver productos disponibles
  ↓
Seleccionar producto
  ↓
Ver detalle, precio y formato
  ↓
Elegir cantidad
  ↓
Agregar al carrito
  ↓
Revisar carrito
  ↓
Confirmar productos y cantidades
  ↓
Enviar pedido por WhatsApp
  ↓
Coordinar pago y despacho con el emprendimiento
```

### Flujo 2: búsqueda y lectura de contenido

```text
Inicio
  ↓
Blog
  ↓
Buscar artículo o elegir categoría
  ↓
Ver listado de artículos
  ↓
Seleccionar artículo
  ↓
Leer contenido
  ↓
Compartir artículo o visitar un producto relacionado
```

### Flujo 3: contacto y consulta

```text
Inicio
  ↓
Contacto o Preguntas frecuentes
  ↓
Consultar información
  ↓
Seleccionar WhatsApp o Instagram
  ↓
Enviar consulta
  ↓
Recibir respuesta del emprendimiento
```

## Categorías

> Guía: [Categorías de productos y temas del blog](../evaluacion/guias/fase-1-requerimientos/07-categorias.md)

### Categorías de productos

| Categoría | Productos |
|---|---|
| Huevos | Huevos por unidad, bandeja o caja, según los formatos disponibles. |
| Frutos secos | Nueces, almendras y otros frutos secos disponibles. |
| Mermeladas y manjar | Mermeladas y manjar artesanal. |
| Otros productos | Productos adicionales disponibles según temporada y stock. |

### Categorías del blog

| Categoría | Idea de artículo | Necesidad o motivación de la proto-persona | Producto relacionado |
|---|---|---|---|
| Alimentación | ¿Cómo saber si un huevo está fresco? | Elegir productos de buena calidad. | Huevos |
| Consejos y recomendaciones | ¿Cómo conservar correctamente los huevos? | Mantener los productos en buenas condiciones. | Huevos |
| Recetas | 5 ideas de desayunos fáciles con huevos | Preparar comidas prácticas para el hogar. | Huevos |
| Alimentación | Beneficios de incorporar frutos secos a la alimentación | Conocer alternativas para complementar su alimentación. | Frutos secos |
| Recetas | Ideas para disfrutar las mermeladas artesanales | Descubrir nuevas formas de utilizar los productos. | Mermeladas |
| Consejos y recomendaciones | Cómo organizar las compras de productos para el hogar | Ahorrar tiempo y planificar las compras. | Todos los productos |

## Elementos globales de navegación

- **Menú principal:** permite acceder a Inicio, Tienda, Blog, Sobre nosotros y Contacto.
- **Barra de búsqueda:** permite buscar productos y artículos del blog.
- **Acceso al carrito:** permite revisar los productos seleccionados.
- **Botón de WhatsApp:** facilita el contacto y la coordinación de pedidos.
- **Pie de página:** incluye redes sociales, contacto, preguntas frecuentes y políticas.

## Consideraciones de la arquitectura

La página web estará organizada para que los usuarios encuentren fácilmente los productos, conozcan el emprendimiento y accedan a contenido útil a través del blog. La navegación debe ser clara y adaptable a celulares y computadores.

La tienda permitirá explorar productos, consultar precios y preparar pedidos. En esta versión, la confirmación final podrá realizarse por WhatsApp, sin necesidad de implementar inicialmente un sistema de pago online. Las secciones de políticas, despacho y preguntas frecuentes entregarán información importante para generar confianza en los clientes.
