# 🚀 Guía de Despliegue Rápido - C³ Consultoría

## 📦 Preparación

Ya tienes todos los archivos listos en esta carpeta. Solo necesitas subirlos a GitHub.

---

## ✅ MÉTODO 1: Interfaz Web de GitHub (Más Fácil)

### Paso 1: Crear Repositorio

1. Ir a https://github.com/new
2. **Repository name:** `c3-consultoria`
3. **Description:** "Sistema de diagnóstico organizativo para PYMEs y autónomos"
4. **Public** o **Private** (tu elección)
5. ⚠️ **NO marcar** "Add a README file"
6. ⚠️ **NO marcar** "Add .gitignore"
7. ⚠️ **NO marcar** "Choose a license"
8. Hacer clic en **"Create repository"**

### Paso 2: Subir Archivos

1. En la página del repositorio vacío, hacer clic en **"uploading an existing file"**
2. **Arrastrar TODOS los archivos** de esta carpeta a la zona de upload
   - O hacer clic en "choose your files" y seleccionar todos
3. En "Commit changes":
   - Message: `Initial commit - C³ Consultoría website`
   - Description: (opcional)
4. Hacer clic en **"Commit changes"**

### Paso 3: Activar GitHub Pages

1. Ir a **Settings** (engranaje en la parte superior)
2. En el menú lateral, hacer clic en **Pages**
3. En "Build and deployment":
   - **Source:** Deploy from a branch
   - **Branch:** `main` (o `master`)
   - **Folder:** `/ (root)`
4. Hacer clic en **"Save"**

### Paso 4: Esperar y Visitar

1. **Esperar 2-3 minutos** (GitHub necesita construir el sitio)
2. Refrescar la página de Settings → Pages
3. Verás un mensaje verde: **"Your site is live at"**
4. Tu sitio estará en:
   ```
   https://TU-USUARIO.github.io/c3-consultoria/
   ```

---

## ✅ MÉTODO 2: Git desde Terminal (Avanzado)

### Requisitos previos:
- Git instalado
- Cuenta de GitHub

### Comandos:

```bash
# Navegar a esta carpeta
cd /ruta/a/esta/carpeta

# Inicializar repositorio Git
git init

# Añadir todos los archivos
git add .

# Hacer el primer commit
git commit -m "Initial commit - C³ Consultoría website"

# Conectar con GitHub (reemplaza TU-USUARIO)
git remote add origin https://github.com/TU-USUARIO/c3-consultoria.git

# Renombrar rama a main
git branch -M main

# Subir archivos
git push -u origin main
```

Luego ir a Settings → Pages y activar como en el Método 1, Paso 3.

---

## 🔧 Configuración Post-Despliegue

### 1. Configurar Web3Forms (OBLIGATORIO)

Para que los formularios funcionen:

1. Ir a https://web3forms.com
2. Ingresar email: `camino.chus@gmail.com`
3. Obtener Access Key
4. Editar estos archivos en GitHub:
   - `index.html`
   - `Cuestionario_Autonomos_sin_trabajadores.html`
   - `Cuestionario_Autonomos_con_trabajadores.html`
   - `Cuestionario_basic_PYME.html`
5. Buscar: `TU_WEB3FORMS_ACCESS_KEY_AQUI`
6. Reemplazar con tu Access Key
7. Commit: "Configure Web3Forms"

### 2. Verificar Funcionamiento

- [ ] Landing page carga
- [ ] Cuestionarios abren
- [ ] Documentos legales abren
- [ ] Formulario de contacto envía
- [ ] Banner de cookies funciona
- [ ] Responsive en móvil

---

## 🌍 Dominio Personalizado (Opcional)

Si tienes un dominio propio (ej: `www.c3consultoria.com`):

### En tu proveedor de dominios:

1. Crear registro **CNAME**:
   - Host: `www`
   - Value: `TU-USUARIO.github.io`

2. Crear registros **A** (si quieres apex domain):
   ```
   185.199.108.153
   185.199.109.153
   185.199.110.153
   185.199.111.153
   ```

### En GitHub:

1. Settings → Pages → Custom domain
2. Ingresar: `www.c3consultoria.com`
3. Save
4. Marcar: "Enforce HTTPS"

### En el código:

1. Editar `CNAME`:
   ```
   www.c3consultoria.com
   ```
2. Commit y push

---

## 📊 Analíticas (Opcional)

### Google Analytics:

1. Crear cuenta en https://analytics.google.com
2. Obtener tu Tracking ID (ej: `G-XXXXXXXXXX`)
3. Añadir al final de `<head>` en `index.html`:

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXXXXX');
</script>
```

---

## 🔄 Actualizaciones Futuras

Para actualizar el sitio:

### Desde la web:
1. Ir al archivo en GitHub
2. Hacer clic en el lápiz (Edit)
3. Hacer cambios
4. Commit changes
5. Esperar 1-2 minutos

### Desde Git:
```bash
git add .
git commit -m "Descripción del cambio"
git push
```

---

## 🐛 Solución de Problemas

### El sitio no aparece después de 5 minutos:
1. Settings → Pages → Verificar que esté activado
2. Actions → Ver si hay errores en el build
3. Verificar que `index.html` esté en la raíz

### Error 404 en cuestionarios:
- Verificar que los nombres de archivo NO tengan espacios
- Verificar que las mayúsculas/minúsculas coincidan

### Formularios no envían:
- Verificar que hayas configurado Web3Forms Access Key
- Verificar en la consola del navegador (F12)

### Banner de cookies no aparece:
- Limpiar cookies del navegador
- Abrir en modo incógnito

---

## 📞 Soporte

**C³ Consultoría Estratégica**
- 📧 Email: camino.chus@gmail.com
- 📋 GitHub Issues: En tu repositorio → Issues

---

## ✅ Checklist Final

- [ ] Repositorio creado en GitHub
- [ ] Todos los archivos subidos
- [ ] GitHub Pages activado
- [ ] Sitio accesible en la URL
- [ ] Web3Forms configurado
- [ ] Formularios probados
- [ ] Cuestionarios probados
- [ ] Mobile responsive verificado
- [ ] Sin errores en consola
- [ ] README.md actualizado con tu URL

---

🎉 **¡Tu sitio está en vivo!**

**URL:** `https://TU-USUARIO.github.io/c3-consultoria/`
