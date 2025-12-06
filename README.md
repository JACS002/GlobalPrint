# 🖨️ GlobalPrint

![GlobalPrint Banner](assets/Logo%20compacto@2x-8.png)

## Descripción

GlobalPrint es un sitio web corporativo diseñado para una empresa de impresión profesional que ofrece servicios integrales de impresión digital, offset, gran formato, papelería corporativa, formularios y etiquetas. El proyecto presenta una interfaz moderna y responsive que destaca los servicios de la empresa y facilita el contacto con los clientes.

## Características Principales

- **Diseño Responsivo**: Adaptable a dispositivos móviles, tablets y escritorio
- **Navegación Intuitiva**: Menú sticky con acceso rápido a todas las secciones
- **Hero Section con Video**: Página de inicio impactante con video de fondo
- **Catálogo de Productos**: Galería interactiva de servicios de impresión
- **Formulario de Contacto**: Integración con Formspree para cotizaciones
- **Animaciones Suaves**: Efectos visuales con WOW.js y Animate.css
- **Carrusel de Imágenes**: Showcase de trabajos realizados
- **Footer Informativo**: Links rápidos y información de contacto

## Tecnologías Utilizadas

### Frontend
- **HTML5**: Estructura semántica del sitio web
- **CSS3**: Estilos personalizados y diseño responsive
- **JavaScript**: Interactividad y funcionalidad dinámica

### Frameworks y Librerías
- **Bootstrap 4.6.2**: Framework CSS para diseño responsive
  - Grid system
  - Componentes de navegación
  - Utilidades de espaciado
- **jQuery 3.5.1**: Manipulación del DOM (requerido por Bootstrap)
- **WOW.js**: Biblioteca para animaciones al hacer scroll
- **Animate.css 4.1.1**: Colección de animaciones CSS
- **Font Awesome 6.5.2**: Iconos vectoriales y logos sociales
- **SweetAlert2**: Alertas modales elegantes (página de contactos)

### Fuentes
- **Google Fonts - Montserrat**: Familia tipográfica principal con múltiples pesos
  - Montserrat Light
  - Montserrat Semi-Light
  - Montserrat Medium
  - Montserrat Bold

### Servicios Externos
- **Formspree**: Servicio de procesamiento de formularios sin backend

### Control de Versiones
- **Git**: Sistema de control de versiones

## Estructura del Proyecto

```
GlobalPrint/
│
├── index.html                    # Página de inicio
├── nosotros.html                 # Página sobre la empresa
├── productos.html                # Catálogo de productos
├── contactos.html                # Formulario de contacto
├── fotoAutores.html             # Créditos de imágenes
├── README.md                     # Documentación del proyecto
├── wow.min.js                   # Librería WOW.js
│
├── assets/                       # Recursos multimedia
│   ├── Logo compacto@2x-8.png
│   ├── isotipo@2x-8.png
│   ├── gif home.mp4
│   ├── fondodescripcionhome.jpg
│   ├── carrusel1.jpg
│   ├── carrusel2.jpg
│   ├── carrusel3.jpg
│   ├── impresiondigital1.jpg
│   ├── impresionoffset1.jpg
│   ├── impresioGranFormato1.jpg
│   ├── papeleriacorporativa3.jpg
│   ├── formularios1.jpg
│   └── etiquetas1.jpg
│
├── css/                          # Hojas de estilo
│   ├── home.css
│   ├── nosotros.css
│   ├── productos.css
│   ├── contactos.css
│   └── seccion-productos/
│       ├── etiquetas.css
│       ├── formulariosVarios.css
│       ├── impresionDigital.css
│       ├── impresionGranFormato.css
│       ├── impresionOffset.css
│       └── PapeleriaCorporativa.css
│
└── seccion-Productos/            # Páginas de detalle de productos
    ├── etiquetas.html
    ├── formulariosVarios.html
    ├── impresionDigital.html
    ├── impresionGranFormato.html
    ├── impresionOffset.html
    └── PapeleriaCorporativa.html
```

## Páginas del Sitio

### 1. **Inicio (index.html)**
- Hero section con video de fondo
- Descripción de la empresa
- Características del equipo
- Footer con enlaces rápidos

### 2. **Nosotros (nosotros.html)**
- Información corporativa
- Carrusel de imágenes
- Historia, misión y visión de la empresa

### 3. **Productos (productos.html)**
- Grid de 6 categorías de productos:
  - Impresión digital
  - Impresión offset
  - Impresión gran formato
  - Papelería corporativa
  - Formularios varios
  - Etiquetas

### 4. **Contactos (contactos.html)**
- Información de contacto
- Horarios de atención
- Formulario de cotización integrado con Formspree
- Alertas con SweetAlert2

### 5. **Secciones de Productos**
Páginas individuales para cada categoría de producto con detalles específicos.

## Funcionalidades Destacadas

### Navegación Activa
El navbar destaca la página actual con un color azul distintivo mediante la clase `.nav-activado`.

### Animaciones
- **WOW.js**: Detecta cuando los elementos entran en el viewport
- **Animate.css**: Proporciona las animaciones (fadeIn, slideInDown, slideInUp)
- Delays personalizados para efectos secuenciales

### Video de Hero
```html
<video autoplay loop muted playsinline class="back-video">
  <source src="assets/gif home.mp4" type="video/mp4">
</video>
```
- `autoplay`: Reproduce automáticamente
- `loop`: Reproducción continua
- `muted`: Sin sonido para permitir autoplay
- `playsinline`: Reproducción inline en dispositivos móviles

### Formulario de Contacto
Integrado con Formspree para envío de correos sin necesidad de backend:
```html
<form action="https://formspree.io/f/xdoqjwrg" method="POST">
```

### Responsive Design
Media queries para diferentes dispositivos:
- **Mobile**: < 768px
- **Tablet**: 768px - 1024px
- **Desktop**: > 1024px

## Instalación y Uso

### Requisitos Previos
- Navegador web moderno (Chrome, Firefox, Safari, Edge)
- Editor de código (VSCode recomendado)
- Servidor local (opcional, puede abrirse directamente)

### Instalación

1. **Clonar el repositorio**
```bash
git clone <URL_DEL_REPOSITORIO>
cd GlobalPrint
```

2. **Abrir el proyecto**
```bash
# Con VSCode
code .

# O con Live Server
# Click derecho en index.html > Open with Live Server
```

3. **Abrir en el navegador**
- Simplemente abre `index.html` en tu navegador
- O usa un servidor local como Live Server de VSCode

### Sin Instalación
El sitio es estático y puede abrirse directamente haciendo doble clic en `index.html`.

## Compatibilidad

- ✅ Chrome (últimas 2 versiones)
- ✅ Firefox (últimas 2 versiones)
- ✅ Safari (últimas 2 versiones)
- ✅ Edge (últimas 2 versiones)
- ✅ Dispositivos móviles iOS y Android

## Paleta de Colores

- **Naranja Principal**: `#E6540F`
- **Azul Principal**: `#366bd4`
- **Fondo Oscuro**: `#343a40`
- **Texto Principal**: `#000000`
- **Texto Claro**: `#ffffff`

## Créditos

Para créditos de las imágenes utilizadas, visita la página [Autores de Fotos](fotoAutores.html).

---

