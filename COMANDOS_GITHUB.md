# 🚀 Comandos Listos para Subir a GitHub

## ✅ Ya está todo configurado!

Todos los archivos están listos. Solo necesitas ejecutar estos comandos:

---

## 📝 PASO 1: Hacer el Commit

Copia y pega este comando en PowerShell:

```powershell
cd "c:\USFQ Sexto Semestre\Desarrollo Web 1\GlobalPrint"
git commit -m "Initial commit - Proyecto GlobalPrint sanitizado para portafolio académico

- Versión sanitizada con datos ficticios
- Archivos originales protegidos con .gitignore
- Proyecto académico USFQ - Desarrollo Web 1
- Formularios desactivados para demostración
- README con disclaimer de privacidad"
```

---

## 📝 PASO 2: Crear Repositorio en GitHub

1. Ve a: https://github.com/new
2. Configura así:
   - **Repository name:** `globalprint-portfolio`
   - **Description:** `Sitio web corporativo de imprenta - Proyecto académico USFQ Desarrollo Web 1`
   - **Visibilidad:** Público (recomendado para portafolio)
   - **NO marques:** "Add a README file"
   - **NO marques:** "Add .gitignore"
   - **NO marques:** "Choose a license"

3. Click en "Create repository"

---

## 📝 PASO 3: Conectar y Subir

**⚠️ IMPORTANTE:** Reemplaza `TU_USUARIO` con tu nombre de usuario de GitHub

```powershell
cd "c:\USFQ Sexto Semestre\Desarrollo Web 1\GlobalPrint"
git remote add origin https://github.com/TU_USUARIO/globalprint-portfolio.git
git branch -M main
git push -u origin main
```

### Ejemplo:
Si tu usuario es `juanperez`, el comando sería:
```powershell
git remote add origin https://github.com/juanperez/globalprint-portfolio.git
```

---

## 📝 PASO 4: Verificación en GitHub

Después del push, ve a tu repositorio en GitHub y verifica:

✅ **Deberías ver:**
- Archivos con sufijo `-sanitized.html`
- README-sanitized.md (como principal)
- Carpetas: `assets/`, `css/`, `seccion-Productos/`
- Archivos: `.gitignore`, `GUIA_USO.md`, `wow.min.js`

❌ **NO deberías ver:**
- `index.html` (sin -sanitized)
- `contactos.html` (sin -sanitized)
- `README.md` (sin -sanitized)
- Ningún archivo original con datos reales

---

## 📝 PASO 5: Configurar GitHub Pages (Opcional)

Si quieres que tu sitio sea accesible en línea:

1. En tu repositorio de GitHub, ve a **Settings**
2. En el menú izquierdo, click en **Pages**
3. En "Branch", selecciona **main**
4. Click en **Save**
5. Espera unos minutos
6. Tu sitio estará en: `https://TU_USUARIO.github.io/globalprint-portfolio/index-sanitized.html`

---

## 🔄 Comandos para Actualizaciones Futuras

Cuando hagas cambios a los archivos sanitizados:

```powershell
cd "c:\USFQ Sexto Semestre\Desarrollo Web 1\GlobalPrint"
git add .
git commit -m "Descripción de los cambios"
git push
```

---

## 🆘 Solución de Problemas

### Problema: "remote origin already exists"
```powershell
git remote remove origin
git remote add origin https://github.com/TU_USUARIO/globalprint-portfolio.git
```

### Problema: Git pide usuario y contraseña
- Usa un **Personal Access Token** en lugar de contraseña
- Genera uno en: https://github.com/settings/tokens
- Permisos necesarios: `repo`

### Problema: "failed to push"
```powershell
git pull origin main --allow-unrelated-histories
git push -u origin main
```

---

## 📊 Resumen de lo que SE SUBE

```
✅ 39 archivos en total:
   - 13 archivos sanitizados (.html y .md)
   - 16 assets (imágenes y video)
   - 10 archivos CSS
   - 3 archivos de configuración/documentación
   - 0 archivos con datos reales (protegidos)
```

---

## ⚠️ ÚLTIMA VERIFICACIÓN antes del Push

Ejecuta esto para estar 100% seguro:

```powershell
cd "c:\USFQ Sexto Semestre\Desarrollo Web 1\GlobalPrint"
Write-Host "`n=== VERIFICACIÓN FINAL ===" -ForegroundColor Cyan
Write-Host "`nArchivos que SE SUBIRÁN:" -ForegroundColor Green
git ls-files | Where-Object { $_ -match "-sanitized" } | Measure-Object | ForEach-Object { Write-Host "  Archivos sanitizados: $($_.Count)" }
Write-Host "`nArchivos que NO se subirán (protegidos):" -ForegroundColor Yellow
@('index.html','contactos.html','nosotros.html','productos.html','README.md') | ForEach-Object {
    if (!(git ls-files $_)) { Write-Host "  ✅ $_ - PROTEGIDO" -ForegroundColor Green }
    else { Write-Host "  ❌ $_ - EN GIT (PROBLEMA!)" -ForegroundColor Red }
}
```

Si todos muestran ✅, ¡estás listo para el push!

---

## 🎯 Todo en Una Línea (Método Rápido)

Si ya creaste el repositorio en GitHub, copia TODA esta línea:

```powershell
cd "c:\USFQ Sexto Semestre\Desarrollo Web 1\GlobalPrint"; git commit -m "Initial commit - GlobalPrint sanitizado"; git remote add origin https://github.com/TU_USUARIO/globalprint-portfolio.git; git branch -M main; git push -u origin main
```

**⚠️ Recuerda cambiar `TU_USUARIO`!**

---

## 📱 Cómo Compartir tu Proyecto

Una vez subido, puedes compartir:

**URL del Repositorio:**
```
https://github.com/TU_USUARIO/globalprint-portfolio
```

**URL del Sitio (si activaste GitHub Pages):**
```
https://TU_USUARIO.github.io/globalprint-portfolio/index-sanitized.html
```

**En tu CV/LinkedIn:**
```
Proyecto Web: GlobalPrint
Sitio corporativo responsive con Bootstrap, animaciones CSS y formularios.
Ver código: github.com/TU_USUARIO/globalprint-portfolio
```

---

## ✅ Checklist Final

Antes de cerrar esta ventana:

- [ ] Hice el commit
- [ ] Creé el repositorio en GitHub
- [ ] Conecté el remote origin
- [ ] Hice el push
- [ ] Verifiqué en GitHub que solo hay archivos sanitizados
- [ ] (Opcional) Configuré GitHub Pages
- [ ] Guardé la URL de mi repositorio

---

**¡Listo! Tu proyecto está seguro en GitHub** 🎉

Archivos originales: 🔒 Seguros en tu PC  
Archivos públicos: ✅ En GitHub para tu portafolio
