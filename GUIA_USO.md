# 📚 Guía de Uso - GlobalPrint

## 🔐 Sistema de Archivos Duales

Este proyecto utiliza un sistema de **archivos duales** para mantener la privacidad:

### Archivos Originales (Privados)
- Contienen información real de contacto
- **NO se suben** al repositorio público
- Solo para uso local/desarrollo

### Archivos Sanitizados (Públicos)
- Terminan con `-sanitized.html` o `-sanitized.md`
- Contienen datos ficticios
- **SON los que se suben** a GitHub
- Para portafolio y demostración

## 📂 Estructura de Archivos

```
ARCHIVO ORIGINAL          →  ARCHIVO SANITIZADO (público)
───────────────────────────────────────────────────────
index.html                →  index-sanitized.html
nosotros.html             →  nosotros-sanitized.html
productos.html            →  productos-sanitized.html
contactos.html            →  contactos-sanitized.html
fotoAutores.html          →  fotoAutores-sanitized.html
README.md                 →  README-sanitized.md

seccion-Productos/:
  impresionDigital.html   →  impresionDigital-sanitized.html
  impresionOffset.html    →  impresionOffset-sanitized.html
  [y así sucesivamente...]
```

## 🎯 Cómo Usar

### Para Desarrollo Local (con datos reales)
1. Abre los archivos **sin** el sufijo `-sanitized`
2. Ejemplo: `index.html`, `contactos.html`
3. Estos archivos tienen la información real

### Para Publicación/Portafolio (datos ficticios)
1. Abre los archivos **con** el sufijo `-sanitized`
2. Ejemplo: `index-sanitized.html`, `contactos-sanitized.html`
3. Estos archivos tienen datos ficticios seguros

## 🚀 Subir a GitHub

### Paso 1: Inicializar Git
```bash
cd "c:\USFQ Sexto Semestre\Desarrollo Web 1\GlobalPrint"
git init
```

### Paso 2: Verificar qué se subirá
```bash
git status
```

Deberías ver:
- ✅ Archivos `-sanitized.html` y `-sanitized.md`
- ✅ Carpetas `assets/` y `css/`
- ✅ Archivo `.gitignore`
- ❌ **NO** deberías ver los archivos originales (.html sin sufijo)

### Paso 3: Agregar archivos
```bash
git add .
```

### Paso 4: Hacer commit
```bash
git commit -m "Initial commit - Versión sanitizada para portafolio"
```

### Paso 5: Conectar con GitHub
```bash
# Crea un repositorio en GitHub primero
git remote add origin https://github.com/TU_USUARIO/globalprint.git
git branch -M main
git push -u origin main
```

## ⚠️ Verificación de Seguridad

Antes de hacer push, verifica:

```bash
# Ver qué archivos están siendo trackeados
git ls-files
```

Asegúrate de que **NO** aparezcan:
- ❌ `index.html` (sin -sanitized)
- ❌ `contactos.html` (sin -sanitized)
- ❌ `README.md` (sin -sanitized)
- ❌ Cualquier archivo con datos reales

## 🔄 Actualizar Archivos Sanitizados

Si haces cambios en los archivos originales y necesitas actualizarlos en las versiones sanitizadas:

### Opción 1: Manualmente
1. Copia el contenido del archivo original
2. Pégalo en el archivo `-sanitized`
3. Reemplaza manualmente los datos reales por ficticios

### Opción 2: Automatizada (PowerShell)
```powershell
# Regenerar archivo sanitizado específico
Get-Content "index.html" | ForEach-Object { 
    $_ -replace 'gp\.ec@hotmail\.com', 'contacto@globalprint-demo.com' `
       -replace '593980840329', '593999999999' `
       -replace '098 084-0329', '+593 99 999-9999' `
       -replace '023228683', '029999999' `
       -replace '02 322-8683', '02 999-9999'
} | Set-Content "index-sanitized.html"
```

## 📝 Datos Ficticios Usados

Para consistencia, usa siempre estos valores en versiones sanitizadas:

| Tipo | Original (NO PUBLICAR) | Ficticio (PUBLICAR) |
|------|------------------------|---------------------|
| Email | gp.ec@hotmail.com | contacto@globalprint-demo.com |
| WhatsApp | 098 084-0329 | +593 99 999-9999 |
| Teléfono | 02 322-8683 | 02 999-9999 |
| Formspree | https://formspree.io/f/xdoqjwrg | # (desactivado) |

## 🛡️ Checklist Pre-Publicación

Antes de hacer `git push`:

- [ ] Verificar que `.gitignore` está configurado correctamente
- [ ] Confirmar que solo archivos `-sanitized` serán subidos
- [ ] Revisar que no hay datos reales en archivos sanitizados
- [ ] Verificar que el formulario está desactivado
- [ ] Comprobar que README-sanitized.md tiene el disclaimer
- [ ] Hacer un `git status` para confirmar archivos

## 📧 Soporte

Si tienes dudas sobre qué archivos subir o cómo mantener la privacidad, revisa:
1. Este archivo (`GUIA_USO.md`)
2. El archivo `.gitignore`
3. El disclaimer en `README-sanitized.md`

## 🎓 Recordatorio

Este es un proyecto **ACADÉMICO**. Los archivos sanitizados son para:
- ✅ Portafolio público
- ✅ Demostración de habilidades
- ✅ Compartir con empleadores

Los archivos originales son para:
- ✅ Desarrollo local
- ✅ Trabajo real con el cliente
- ❌ **NUNCA para repositorios públicos**

---

**Mantén tu información segura y tu portafolio profesional** 🔒✨
