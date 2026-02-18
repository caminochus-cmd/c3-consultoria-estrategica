# C³ Consultoría Estratégica 🏢

[![GitHub Pages](https://img.shields.io/badge/GitHub-Pages-blue?logo=github)](https://github.com)
[![License](https://img.shields.io/badge/License-Proprietary-red.svg)]()
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)]()
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)]()
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)]()

## 📋 Descripción

Sistema de diagnóstico organizativo para PYMEs y autónomos basado en cuestionarios de madurez con **106 preguntas** y recomendaciones asistidas por IA.

**Metodología · Coherencia · Satisfacción**

---

## 🌐 Demo en Vivo

**URL del sitio:** `https://TU-USUARIO.github.io/c3-consultoria/`

*(Reemplaza `TU-USUARIO` con tu usuario de GitHub)*

---

## 📦 Contenido del Proyecto

### 🏠 Landing Page
- `index.html` - Página principal con todas las secciones
  - Hero con propuesta de valor
  - Sección "El Problema"
  - Valores corporativos
  - Catálogo de servicios
  - Casos de uso
  - Diferenciadores competitivos
  - Acceso a cuestionarios
  - Formulario de contacto
  - Acordeones legales en footer

### 📋 Cuestionarios de Madurez (3)
- `Cuestionario_Autonomos_sin_trabajadores.html` - 106 preguntas para profesionales independientes
- `Cuestionario_Autonomos_con_trabajadores.html` - 106 preguntas + gestión de equipo
- `Cuestionario_basic_PYME.html` - 106 preguntas enfoque directivo

**Características de los cuestionarios:**
- ✅ Escala Likert 1-5
- ✅ 3 fases de diagnóstico
- ✅ Guardado automático (localStorage)
- ✅ Exportación a PDF
- ✅ Exportación a Excel/Google Sheets
- ✅ Envío por email a C³
- ✅ Soporte de voz en 7 idiomas
- ✅ Barra de progreso
- ✅ Estadísticas en tiempo real

### ⚖️ Documentos Legales (3)
- `politica-privacidad.html` - RGPD + LOPDGDD + AI Act
- `aviso-legal.html` - LSSI + AI Act + PI
- `politica-cookies.html` - Gestión de consentimiento granular

### 📄 Documentación
- `docs/snippet-banner-cookies.html` - Banner de cookies reutilizable
- `README.md` - Este archivo

---

## 🚀 Despliegue en GitHub Pages

### Opción 1: Desde la Interfaz Web (Recomendado)

1. **Crear repositorio:**
   - Ir a https://github.com/new
   - Nombre: `c3-consultoria`
   - Público o Privado (tu elección)
   - ✅ NO inicializar con README (ya lo tienes)

2. **Subir archivos:**
   - Hacer clic en "uploading an existing file"
   - Arrastrar todos los archivos de esta carpeta
   - Commit: "Initial commit - C³ website"

3. **Activar GitHub Pages:**
   - Ir a Settings → Pages
   - Source: Deploy from a branch
   - Branch: `main` / `root`
   - Save

4. **Esperar 2-3 minutos** y visitar:
   ```
   https://TU-USUARIO.github.io/c3-consultoria/
   ```

### Opción 2: Desde Git (Línea de comandos)

```bash
# Inicializar repositorio
git init
git add .
git commit -m "Initial commit - C³ Consultoría website"

# Conectar con GitHub
git remote add origin https://github.com/TU-USUARIO/c3-consultoria.git
git branch -M main
git push -u origin main

# Activar GitHub Pages desde Settings → Pages
```

---

## 📧 Configuración de Formularios

### ⚠️ IMPORTANTE: Configurar Web3Forms

Los formularios están configurados con **Web3Forms** para envío de emails.

**Pasos (5 minutos):**

1. **Obtener Access Key:**
   - Ir a https://web3forms.com
   - Ingresar email: `camino.chus@gmail.com`
   - Copiar el Access Key

2. **Reemplazar en los archivos:**
   
   **En los 3 cuestionarios**, buscar:
   ```javascript
   access_key: "TU_WEB3FORMS_ACCESS_KEY_AQUI",
   ```
   
   **En `index.html`**, buscar:
   ```html
   <input type="hidden" name="access_key" value="TU_WEB3FORMS_ACCESS_KEY_AQUI">
   ```
   
   Reemplazar con tu Access Key real.

3. **Commit y push:**
   ```bash
   git add .
   git commit -m "Configure Web3Forms access key"
   git push
   ```

---

## 🎨 Paleta de Colores C³

```css
--dorado-c3:      #B8860B  /* Dorado corporativo */
--dorado-oscuro:  #8B6914  /* Dorado oscuro */
--negro:          #2C2C2C  /* Negro corporativo */
--gris:           #6B6B6B  /* Gris cálido */
--beige:          #FAF8F5  /* Beige fondo */
--beige-borde:    #D4C5A9  /* Beige bordes */
--blanco:         #FFFFFF  /* Blanco puro */
```

---

## 🛠️ Estructura de Archivos

```
c3-consultoria/
├── index.html                                    # Landing page principal
├── Cuestionario_Autonomos_sin_trabajadores.html
├── Cuestionario_Autonomos_con_trabajadores.html
├── Cuestionario_basic_PYME.html
├── politica-privacidad.html
├── aviso-legal.html
├── politica-cookies.html
├── docs/
│   └── snippet-banner-cookies.html
├── css/
│   └── (vacío - CSS integrado en HTML)
├── js/
│   └── (vacío - JS integrado en HTML)
├── img/
│   └── (vacío - SVG inline)
├── README.md
├── LICENSE
└── .gitignore
```

---

## 🔒 Seguridad y Privacidad

- ✅ **RGPD completo** con 11 secciones
- ✅ **LOPDGDD** - Ley Orgánica española
- ✅ **AI Act** - Transparencia algorítmica
- ✅ **LSSI** - Art. 10 cumplido
- ✅ **ePrivacy** - Gestión de cookies granular
- ✅ **Canal ARCO-POL** - privacidad@c3consultoria.es

---

## 📊 Tecnologías

- **HTML5** - Estructura semántica
- **CSS3** - Variables CSS, Grid, Flexbox
- **JavaScript ES6+** - Vanilla JS (sin frameworks)
- **Web3Forms** - Envío de formularios sin backend
- **LocalStorage** - Guardado automático de progreso
- **Web Speech API** - Reconocimiento de voz
- **jsPDF + autoTable** - Generación de PDFs
- **SheetJS (xlsx)** - Exportación a Excel

---

## 🌍 Compatibilidad de Navegadores

| Navegador | Versión Mínima | Soporte |
|-----------|----------------|---------|
| Chrome    | 90+            | ✅ Completo |
| Firefox   | 88+            | ✅ Completo |
| Safari    | 14+            | ✅ Completo |
| Edge      | 90+            | ✅ Completo |
| Opera     | 76+            | ✅ Completo |

---

## 📱 Responsive Design

- ✅ Desktop (1920px+)
- ✅ Laptop (1366px - 1920px)
- ✅ Tablet (768px - 1366px)
- ✅ Mobile (320px - 768px)

---

## 🧪 Testing

### Checklist de Validación:

- [ ] Landing page carga correctamente
- [ ] Los 3 cuestionarios abren desde la landing
- [ ] Los 3 documentos legales abren en nueva pestaña
- [ ] Acordeones legales del footer funcionan
- [ ] Banner de cookies aparece y funciona
- [ ] Formulario de contacto envía emails
- [ ] Botón "ENVIAR A C³" en cuestionarios funciona
- [ ] Guardado automático en cuestionarios
- [ ] Exportación a PDF funciona
- [ ] Exportación a Excel funciona
- [ ] Responsive en móvil
- [ ] No hay errores en consola del navegador

---

## 📞 Contacto

**C³ Consultoría Estratégica**
- 📧 Email: camino.chus@gmail.com
- 📧 Privacidad: privacidad@c3consultoria.es
- 🌐 Web: [https://tu-usuario.github.io/c3-consultoria/](URL del sitio)
- 📍 Ubicación: Barcelona, España

---

## 📄 Licencia

**Propietario:** C³ Consultoría Estratégica  
**Todos los derechos reservados © 2025**

Este proyecto contiene material propietario de C³ Consultoría. 
No se permite el uso comercial sin autorización expresa.

---

## 🔄 Actualizaciones

### v1.0 (Febrero 2025)
- ✅ Landing page completa con 7 secciones
- ✅ 3 cuestionarios de madurez (106 preguntas c/u)
- ✅ 3 documentos legales (RGPD + AI Act + LSSI)
- ✅ Banner de cookies con consentimiento granular
- ✅ Formularios con envío por email
- ✅ Exportación PDF y Excel
- ✅ Soporte de voz en 7 idiomas
- ✅ Acordeones legales en footer

---

## 🤝 Contribuciones

Este es un proyecto privado de C³ Consultoría Estratégica.

---

## ⭐ Características Destacadas

- 🎯 **Sistema de diagnóstico completo** con 106 preguntas validadas
- 🤖 **IA integrada** para análisis de madurez organizativa
- 📊 **Estadísticas en tiempo real** durante el cuestionario
- 💾 **Guardado automático** sin pérdida de progreso
- 📧 **Envío directo por email** sin necesidad de backend
- 🔒 **100% conforme RGPD** con documentación legal completa
- 🎨 **Diseño premium** con paleta corporativa C³
- 📱 **Totalmente responsive** para todos los dispositivos
- 🌐 **Multiidioma** con soporte de voz en 7 idiomas

---

**Desarrollado con ❤️ para PYMEs y autónomos que quieren recuperar el control**

**Metodología • Coherencia • Satisfacción**
