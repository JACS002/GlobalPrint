# 🖨️ GlobalPrint

![GlobalPrint Banner](assets/Logo%20compacto@2x-8.png)

## ⚠️ Disclaimer de Privacidad

> **IMPORTANTE**: Este proyecto fue desarrollado con fines académicos para la materia Desarrollo Web 1 de USFQ (Sexto Semestre). Toda la información de contacto, datos personales y endpoints de servicios han sido **MODIFICADOS** y son **FICTICIOS** para proteger la privacidad. Este repositorio no representa el sitio web oficial de ninguna empresa real y es únicamente un proyecto de demostración educativa.

## 📋 Descripción

GlobalPrint es un sitio web corporativo de demostración diseñado para una empresa ficticia de impresión profesional que ofrece servicios integrales de impresión digital, offset, gran formato, papelería corporativa, formularios y etiquetas. El proyecto presenta una interfaz moderna y responsive que destaca los servicios de la empresa y facilita el contacto con los clientes.

## ✨ Características Principales

- **Diseño Responsivo**: Adaptable a dispositivos móviles, tablets y escritorio
- **Navegación Intuitiva**: Menú sticky con acceso rápido a todas las secciones
- **Hero Section con Video**: Página de inicio impactante con video de fondo
- **Catálogo de Productos**: Galería interactiva de servicios de impresión
- **Formulario de Contacto**: Demo de formulario (desactivado)
- **Animaciones Suaves**: Efectos visuales con WOW.js y Animate.css
- **Carrusel de Imágenes**: Showcase de trabajos realizados
- **Footer Informativo**: Links rápidos y información de contacto

## 🚀 Tecnologías Utilizadas

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

### Control de Versiones
- **Git**: Sistema de control de versiones

## 📁 Estructura del Proyecto

```
GlobalPrint/
│
├── *-sanitized.html              # Versiones públicas (datos ficticios)
├── *.html                        # Archivos originales (NO en repositorio público)
├── README-sanitized.md           # Documentación pública
├── README.md                     # Documentación original (NO en repositorio público)
├── wow.min.js                   # Librería WOW.js
│
├── assets/                       # Recursos multimedia
│   ├── Logo compacto@2x-8.png
│   ├── isotipo@2x-8.png
│   ├── gif home.mp4
│   └── [imágenes...]
│
├── css/                          # Hojas de estilo
│   ├── home.css
│   ├── nosotros.css
│   ├── productos.css
│   └── contactos.css
│
└── seccion-Productos/            # Páginas de detalle de productos
    ├── *-sanitized.html          # Versiones públicas
    └── *.html                    # Originales (NO en repositorio público)
```

## 🎨 Páginas del Sitio

### 1. **Inicio (index-sanitized.html)**
- Hero section con video de fondo
- Descripción de la empresa
- Características del equipo
- Footer con enlaces rápidos

### 2. **Nosotros (nosotros-sanitized.html)**
- Información corporativa
- Carrusel de imágenes
- Historia, misión y visión de la empresa

### 3. **Productos (productos-sanitized.html)**
- Grid de 6 categorías de productos:
  - Impresión digital
  - Impresión offset
  - Impresión gran formato
  - Papelería corporativa
  - Formularios varios
  - Etiquetas

### 4. **Contactos (contactos-sanitized.html)**
- Información de contacto (ficticia)
- Horarios de atención
- Formulario de cotización (desactivado para demo)

### 5. **Secciones de Productos**
Páginas individuales para cada categoría de producto con detalles específicos.

## 🎯 Funcionalidades Destacadas

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
Configurado para demostración con prevención de envío:
```html
<form action="#" method="POST" onsubmit="event.preventDefault(); alert('Formulario de demostración');">
```
> ⚠️ **Nota**: El formulario ha sido desactivado en esta versión pública para proteger la privacidad.

### Responsive Design
Media queries para diferentes dispositivos:
- **Mobile**: < 768px
- **Tablet**: 768px - 1024px
- **Desktop**: > 1024px

## 🛠️ Instalación y Uso

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

2. **Abrir los archivos sanitizados**
```bash
# Con VSCode
code .

# O con Live Server
# Click derecho en *-sanitized.html > Open with Live Server
```

3. **Abrir en el navegador**
- Abre `index-sanitized.html` en tu navegador
- O usa un servidor local como Live Server de VSCode

### Archivos a Usar
⚠️ **Importante**: Para visualización pública, usa solo los archivos con sufijo `-sanitized.html`

## 📱 Compatibilidad

- ✅ Chrome (últimas 2 versiones)
- ✅ Firefox (últimas 2 versiones)
- ✅ Safari (últimas 2 versiones)
- ✅ Edge (últimas 2 versiones)
- ✅ Dispositivos móviles iOS y Android

## 🎨 Paleta de Colores

- **Naranja Principal**: `#E6540F`
- **Azul Principal**: `#366bd4`
- **Fondo Oscuro**: `#343a40`
- **Texto Principal**: `#000000`
- **Texto Claro**: `#ffffff`

## 📞 Información de Contacto (Ficticia)

> ⚠️ **Los siguientes datos son ficticios y solo para demostración**:

- **Email**: contacto@globalprint-demo.com
- **WhatsApp**: +593 99 999-9999
- **Teléfono**: 02 999-9999
- **Horario**: Lunes a Viernes, 9:00 am - 6:00 pm

## 👥 Créditos

Desarrollado como proyecto académico para la materia de Desarrollo Web 1 - USFQ Sexto Semestre.

Para créditos de las imágenes utilizadas, visita la página [Autores de Fotos](fotoAutores-sanitized.html).

## 📄 Licencia

Este proyecto es de uso académico y demostrativo únicamente.

## 🔒 Nota de Privacidad

- Todos los datos de contacto son ficticios
- El formulario de contacto ha sido desactivado
- Las imágenes y logos son solo para demostración educativa
- Este no es un sitio web comercial real

---

**Proyecto Educativo** - Desarrollado para aprendizaje en diseño y desarrollo web - Universidad San Francisco de Quito (USFQ)
