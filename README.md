[README.md](https://github.com/user-attachments/files/25500958/README.md)
# 🚀 SISTEMA CITRO GOOGLE - VERSIÓN CORREGIDA

Sistema completo de gestión de solicitudes para el H. Consejo Técnico del CITRO.

## ✅ CORRECCIONES APLICADAS

Este paquete incluye todas las correcciones de errores de autenticación:

1. ✅ Client ID corregido (sin "1" extra)
2. ✅ Funciones duplicadas eliminadas
3. ✅ Email de admin corregido
4. ✅ Configuración para solo @gmail.com

## 📦 ARCHIVOS INCLUIDOS

```
citro-sistema-google-CORREGIDO/
├── config-google.js        ✅ CORREGIDO
├── google-auth.js          ✅ CORREGIDO
├── google-drive.js         
├── google-sheets.js        
├── google-gmail.js         
├── app-google.js           
├── forms-data.js           
├── index.html              
├── firebase.json           
└── README.md               
```

## 🎯 ANTES DE EMPEZAR

### 1. Obtener Folder ID de Google Drive

```
1. Ir a https://drive.google.com
2. Crear carpeta "CITRO Solicitudes"
3. Abrir la carpeta
4. Copiar el ID de la URL:
   https://drive.google.com/drive/folders/[COPIAR_ESTE_ID]
```

### 2. Actualizar config-google.js

**Abrir `config-google.js` y cambiar línea 43:**

```javascript
rootFolderId: 'PEGAR_TU_FOLDER_ID_AQUI',
```

## 🚀 INSTALACIÓN (5 MINUTOS)

### PASO 1: Subir a GitHub

```bash
# Crear repositorio en GitHub
# O usar uno existente

cd citro-sistema-google-CORREGIDO

git init
git add .
git commit -m "Sistema CITRO Google v3.0"
git remote add origin https://github.com/TU_USUARIO/citro-sistema-google.git
git push -u origin main
```

### PASO 2: Activar GitHub Pages

```
Settings → Pages
Source: Deploy from a branch
Branch: main
Folder: / (root)
Save
```

**Tu sitio estará en:**
```
https://TU_USUARIO.github.io/citro-sistema-google/
```

### PASO 3: Actualizar Redirect URIs en Google Cloud

```
https://console.cloud.google.com/apis/credentials

Click en tu OAuth Client ID

Authorized JavaScript origins:
  + https://TU_USUARIO.github.io

Authorized redirect URIs:
  + https://TU_USUARIO.github.io/citro-sistema-google/

SAVE
```

### PASO 4: Probar

```
1. Abrir: https://TU_USUARIO.github.io/citro-sistema-google/
2. Click "Continuar con Google"
3. Login con @gmail.com
4. ✅ Debe funcionar
```

## 📊 CONFIGURACIÓN ACTUAL

```javascript
Client ID: 147189238289-c2du7shhgvrd1de9koq17gjb6p2e4bvj...
Spreadsheet ID: 1ZbGK8Nfzp4UTtEyyvlXpYiRfVWxVBTNZvxJw9HMpVMA
Login permitido: Solo @gmail.com
Admins: citroct7@gmail.com, jcfaicus@gmail.com
```

## ⚙️ PERSONALIZAR

### Cambiar dominio permitido

**En `config-google.js` líneas 88-89:**

```javascript
// Solo @gmail.com (actual)
soloEmailUV: true,
dominioPermitido: 'gmail.com',

// Solo @uv.mx
soloEmailUV: true,
dominioPermitido: 'uv.mx',

// Cualquier Google
soloEmailUV: false,
dominioPermitido: '',
```

### Agregar más administradores

**En `config-google.js` líneas 59-62:**

```javascript
admins: [
    'citroct7@gmail.com',
    'jcfaicus@gmail.com',
    'nuevo-admin@gmail.com'  // ← Agregar aquí
],
```

## 🧪 VERIFICAR QUE FUNCIONA

**Abrir consola del navegador (F12):**

```javascript
CONFIG.google.clientId
// Debe mostrar: "147189238289-c2du7shhgvrd1de9koq17gjb6p2e4bvj..."

CONFIG.admins
// Debe mostrar: ["citroct7@gmail.com", "jcfaicus@gmail.com"]

typeof isAdmin
// Debe mostrar: "function"
```

## 📋 CHECKLIST DE INSTALACIÓN

```
□ Obtener Folder ID de Google Drive
□ Actualizar rootFolderId en config-google.js
□ Subir archivos a GitHub
□ Activar GitHub Pages
□ Actualizar Redirect URIs en Google Cloud Console
□ Esperar 3-5 minutos
□ Abrir sitio en ventana privada
□ Ctrl + Shift + R
□ Presionar F12 → Verificar configuración
□ Click "Continuar con Google"
□ ✅ Login funciona
```

## 📚 FORMULARIOS INCLUIDOS

1. **Apoyo Académico** - Congresos, viajes, investigación
2. **Aval Institucional** - Respaldo oficial del CITRO
3. **Apoyo a Terceros** - Colaboradores externos
4. **Comité Tutorial** - Modificaciones de comité (posgrado)
5. **Solicitud Libre** - Otros trámites

## 🆘 SOPORTE

**Si tienes problemas:**

1. Verifica que el Client ID sea correcto
2. Verifica que las Redirect URIs coincidan
3. Verifica el Folder ID de Google Drive
4. Revisa la consola del navegador (F12) para errores

## 📖 DOCUMENTACIÓN

Para más información, consulta:
- Google Cloud Console: https://console.cloud.google.com
- Google Drive: https://drive.google.com
- GitHub Pages: https://pages.github.com

## 🎉 ¡LISTO!

El sistema está completo y listo para usar.

© 2026 - Universidad Veracruzana - CITRO
# GoogldCitro
