# 🏀 Recreación del Logo de Denver Nuggets

## 📋 Descripción del Proyecto

Este tarea recrea el logo oficial de los **Denver Nuggets** utilizando únicamente **HTML5** y **CSS3**, sin el uso de imágenes SVG, Canvas o JavaScript. La recreación incluye todas las características visuales del logo original: círculos concéntricos, hachas cruzadas, montañas y un balón de baloncesto estilizado.

## 🎯 Objetivos del Lab 4

- Recrear una imagen compleja usando solo HTML y CSS
- Implementar **selectores CSS avanzados**
- Utilizar **variables CSS (Custom Properties)**
- Aplicar **CSS Nesting**
- Crear un **sistema de temas intercambiable**
- Desarrollar componentes **totalmente responsivos**

## 🎨 Paleta de Colores

#### Tema Original (Denver Nuggets)
```css
--theme-primary: #FFC627;    /* Amarillo / Dorado */
--theme-secondary: #8B2332;  /* Rojo / Granate */
--theme-tertiary: #0D2240;   /* Azul Marino */
--theme-light: white;        /* Blanco */
```

#### Tema Alternativo
```css
--theme-primary: #4ECDC4;    /* Turquesa */
--theme-secondary: #FF6B6B;  /* Rojo Coral */
--theme-tertiary: #1A535C;   /* Verde Azulado */
--theme-light: #F7FFF7;      /* Blanco Verdoso */
```

## 📂 Estructura del Proyecto

```
Lab4-DenverNuggets/
│
├── index.html          # Estructura HTML del proyecto
├── style.css           # Estilos CSS completos
├── README.md           # Documentación (este archivo)
└── images/
    └── DenverNuggets.png  # Logo original para comparación
```

## 🧩 Componentes del Logo

### 1. **Círculos Concéntricos**
- `.logo-background` - Círculo amarillo exterior
- `.logo-red` - Círculo rojo medio
- `.background` - Círculo azul interior

### 2. **Hachas Cruzadas**
- `.axe-left` - Hacha izquierda con picos y mango
- `.axe-right` - Hacha derecha con picos y mango
- Uso de `clip-path` para formas personalizadas

### 3. **Montañas**
- `.mountain-left` - Montaña blanca (izquierda)
- `.mountain-right` - Montaña amarilla (derecha)

### 4. **Balón de Baloncesto**
- `.basketball` - Contenedor circular
- `.basketball-top` - Mitad superior blanca
- `.basketball-line` - Líneas horizontal y vertical
- `.basketball-curve` - Curvas decorativas

## 📚 Selectores CSS Implementados

El proyecto demuestra el uso de los siguientes selectores CSS:

| Selector | Ejemplo | Uso en el Proyecto |
|----------|---------|-------------------|
| **Descendiente** | `.axe .axe-left-peak-left` | Selección de picos de hacha |
| **Hijo directo** | `ul > li` | Elementos de lista directos |
| **Adyacente** | `.axe-left-peak-left + .axe-left-peak-right` | Segundo pico de hacha |
| **Hermanos** | `.axe-right-peak-left ~ .axe-right-peak-right` | Picos del lado derecho |
| **:first-child** | `ul > li:first-child h3` | Título "Original" |
| **:last-child** | `ul > li:last-child h3` | Título "Recreación" |
| **:nth-child()** | `li:nth-child(2)` | Animación del segundo item |
| **:has()** | `.logo-background:has(.basketball:hover)` | Efecto hover contextual |
| **:checked** | `#theme-toggle:checked` | Estado del botón de tema |
| **::before** | `.logo-background::before` | Gradiente radial |
| **::after** | `.axe-left::after` | Mango de las hachas |

## 🔧 Instalación y Uso

### Servidor Local
```bash
# Usando Python 3
python -m http.server 8000

# Usando Node.js (http-server)
npx http-server

# Acceder en el navegador
http://localhost:8000
```


## 👨‍💻 Autor

Marcelo Detlefsen - 24554