# ⚡ QuizMaster · Trivia App

Una aplicación de preguntas y respuestas con más de 20 categorías, temporizador y sistema de puntuación, construida con React y desplegada en GitHub Pages.

![React](https://img.shields.io/badge/React-18-61dafb?logo=react&logoColor=white&style=flat-square)
![GitHub Pages](https://img.shields.io/badge/GitHub_Pages-deployed-green?logo=github&style=flat-square)
![OpenTDB](https://img.shields.io/badge/API-Open_Trivia_DB-purple?style=flat-square)

---

## ✨ Características

- 🌐 **+20 categorías** de preguntas (ciencia, historia, videojuegos, cine, etc.)
- 🎯 **3 niveles de dificultad**: Fácil, Medio y Difícil
- ⏱ **Temporizador** de 20 segundos por pregunta
- 📊 **Puntuación en tiempo real** con indicador visual
- 📋 **Resumen al final** con todas las respuestas correctas
- 📱 **Diseño responsive** para móvil y escritorio
- 🎨 Interfaz oscura moderna con animaciones suaves

---

## 🚀 Demo en vivo

👉 **[Ver la app en GitHub Pages](https://TU_USUARIO.github.io/trivia-app)**

*(reemplaza `TU_USUARIO` con tu usuario de GitHub una vez desplegado)*

---

## 🛠 Instalación local

### Requisitos previos
- Node.js 16+
- npm 8+

### Pasos

```bash
# 1. Clona el repositorio
git clone https://github.com/TU_USUARIO/trivia-app.git
cd trivia-app

# 2. Instala las dependencias
npm install

# 3. Arranca el servidor de desarrollo
npm start
```

La app se abrirá en [http://localhost:3000](http://localhost:3000)

---

## 📦 Build de producción

```bash
npm run build
```

Genera la carpeta `build/` con todos los archivos optimizados.

---

## 🌐 Despliegue en GitHub Pages

### Primera vez

1. **Crea el repositorio en GitHub** (vacío, sin README)

2. **Edita `package.json`**: cambia la línea `homepage` con tu usuario:
   ```json
   "homepage": "https://TU_USUARIO.github.io/trivia-app"
   ```

3. **Conecta y despliega:**
   ```bash
   git init
   git add .
   git commit -m "🚀 Initial commit"
   git branch -M main
   git remote add origin https://github.com/TU_USUARIO/trivia-app.git
   git push -u origin main

   npm install
   npm run deploy
   ```

4. **Activa GitHub Pages**: Ve a tu repo → Settings → Pages → Source: `gh-pages` branch

### Actualizaciones futuras

```bash
# Hacer cambios, luego:
git add .
git commit -m "descripción del cambio"
git push
npm run deploy
```

---

## 📁 Estructura del proyecto

```
trivia-app/
├── public/
│   └── index.html
├── src/
│   ├── components/
│   │   ├── Home.js / Home.css       # Pantalla de configuración
│   │   ├── Quiz.js / Quiz.css       # Pantalla de juego
│   │   ├── Results.js / Results.css # Pantalla de resultados
│   │   └── Loading.js / Loading.css # Carga y errores
│   ├── constants/
│   │   └── categories.js            # Categorías y configuración
│   ├── utils/
│   │   └── api.js                   # Llamadas a la API de OpenTDB
│   ├── App.js                       # Componente principal
│   ├── index.js                     # Punto de entrada
│   └── index.css                    # Estilos globales y variables
└── package.json
```

---

## 🔌 API

Las preguntas provienen de [Open Trivia Database](https://opentdb.com/), una API gratuita y sin necesidad de autenticación.

Ejemplo de llamada:
```
https://opentdb.com/api.php?amount=10&category=17&difficulty=medium&type=multiple
```

---

## 📄 Licencia

MIT — libre para usar y modificar.
