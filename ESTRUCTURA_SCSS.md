# Estructura SCSS - Arquitectura 7-1 Pattern

Este proyecto utiliza la arquitectura SCSS 7-1 pattern, que organiza los archivos SCSS en 7 carpetas principales más 1 archivo principal.

## 📁 Estructura de Carpetas

```
scss/
├── abstracts/          # Código que no genera CSS (variables, mixins, functions)
│   ├── _variables.scss
│   ├── _mixins.scss
│   └── _functions.scss
├── base/              # Estilos base (reset, tipografía, animaciones)
│   ├── _reset.scss
│   ├── _typography.scss
│   └── _animations.scss
├── layout/            # Componentes de diseño (header, footer, container)
│   ├── _header.scss
│   ├── _footer.scss
│   └── _container.scss
├── components/        # Componentes reutilizables
│   ├── _buttons.scss
│   ├── _cards.scss
│   ├── _forms.scss
│   └── _bootstrap-overrides.scss
├── utilities/         # Utilidades y helpers
│   └── _utilities.scss
└── main.scss          # Archivo principal que importa todos los módulos
```

## 📝 Descripción de Módulos

### Abstracts
- **`_variables.scss`**: Variables SCSS (colores, tipografía, espaciado, breakpoints)
- **`_mixins.scss`**: Mixins reutilizables (media queries, transformaciones, sombras, etc.)
- **`_functions.scss`**: Funciones SCSS (cálculos, conversiones, etc.)

### Base
- **`_reset.scss`**: Reset CSS y estilos base
- **`_typography.scss`**: Estilos de tipografía (títulos, párrafos, etc.)
- **`_animations.scss`**: Definiciones de keyframes y animaciones

### Layout
- **`_header.scss`**: Estilos del header y navegación
- **`_footer.scss`**: Estilos del footer
- **`_container.scss`**: Estilos de contenedores principales

### Components
- **`_buttons.scss`**: Estilos de botones personalizados
- **`_cards.scss`**: Estilos de tarjetas (cards)
- **`_forms.scss`**: Estilos de formularios
- **`_bootstrap-overrides.scss`**: Personalizaciones de componentes Bootstrap

### Utilities
- **`_utilities.scss`**: Clases de utilidad y helpers

## ✨ Características SCSS Implementadas

### Variables
- ✅ Colores (primarios, secundarios, gradientes)
- ✅ Tipografía (fuentes, tamaños, pesos)
- ✅ Espaciado (márgenes, padding)
- ✅ Breakpoints (responsive design)
- ✅ Sombras y efectos

### Mixins
- ✅ Media queries responsive (`@include respond-to()`)
- ✅ Transiciones y transformaciones
- ✅ Sombras y efectos hover
- ✅ Botones con gradientes
- ✅ Efectos shine y ripple
- ✅ Utilidades flexbox y grid

### Funciones
- ✅ Conversión de unidades (px a rem/em)
- ✅ Cálculo de luminosidad y contraste
- ✅ Aclarar/oscurecer colores

### Operadores y Bucles
- ✅ `@for` para generar clases dinámicas (delays de animación, spacing)
- ✅ `@each` para generar utilidades de spacing
- ✅ Operadores matemáticos para cálculos

### Nesting
- ✅ Estructura anidada clara y organizada
- ✅ Uso de `&` para pseudo-clases y modificadores
- ✅ Media queries anidadas

### Extend
- ✅ Uso de `@extend` para compartir estilos comunes (preparado para futuras implementaciones)

### Animaciones y Transiciones
- ✅ Keyframes personalizados (fadeIn, fadeInUp, slideIn, pulse, etc.)
- ✅ Transiciones suaves en elementos interactivos
- ✅ Transformaciones en hover y active
- ✅ Efectos de entrada escalonados

## 🎯 Buenas Prácticas Aplicadas

1. **Nomenclatura**: Uso de guiones bajos para archivos parciales (`_archivo.scss`)
2. **Organización**: Separación clara de responsabilidades por carpetas
3. **Reutilización**: Mixins y variables para evitar repetición
4. **Mantenibilidad**: Código modular y fácil de mantener
5. **Escalabilidad**: Estructura que permite crecer fácilmente
6. **Responsive**: Mobile-first approach con media queries anidadas
7. **Performance**: Uso eficiente de selectores y minimización de repetición

## 📦 Compilación

El archivo `main.scss` importa todos los módulos en el orden correcto:

```scss
@import 'abstracts/variables';
@import 'abstracts/mixins';
@import 'abstracts/functions';
@import 'base/reset';
@import 'base/typography';
@import 'base/animations';
@import 'layout/header';
@import 'layout/footer';
@import 'layout/container';
@import 'components/cards';
@import 'components/buttons';
@import 'components/forms';
@import 'components/bootstrap-overrides';
@import 'utilities/utilities';
```

Para compilar:
```bash
npm run sass
```

Esto genera `css/style.css` que es el archivo que se enlaza en los HTML.


