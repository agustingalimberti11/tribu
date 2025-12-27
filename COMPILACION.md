# Instrucciones de Compilación SCSS

Este proyecto utiliza SCSS (Sass) para la organización de estilos. Para compilar los archivos SCSS a CSS, sigue estos pasos:

## Opción 1: Usando npm (Recomendado)

1. Instala las dependencias:
```bash
npm install
```

2. Compila el SCSS a CSS:
```bash
npm run sass
```

3. Para compilar en modo watch (compila automáticamente cuando cambias archivos):
```bash
npm run sass:watch
```

4. Para compilar en modo comprimido (producción):
```bash
npm run sass:compressed
```

## Opción 2: Instalando Sass globalmente

1. Instala Sass globalmente:
```bash
npm install -g sass
```

2. Compila el SCSS:
```bash
sass scss/main.scss css/style.css --style=expanded
```

3. Modo watch:
```bash
sass --watch scss/main.scss css/style.css --style=expanded
```

## Estructura SCSS

El proyecto sigue la arquitectura 7-1 pattern:

```
scss/
├── abstracts/          # Variables, mixins, functions
│   ├── _variables.scss
│   ├── _mixins.scss
│   └── _functions.scss
├── base/              # Reset, tipografía, animaciones
│   ├── _reset.scss
│   ├── _typography.scss
│   └── _animations.scss
├── layout/            # Header, footer, container
│   ├── _header.scss
│   ├── _footer.scss
│   └── _container.scss
├── components/        # Componentes reutilizables
│   ├── _cards.scss
│   ├── _buttons.scss
│   ├── _forms.scss
│   └── _bootstrap-overrides.scss
├── utilities/         # Utilidades y helpers
│   └── _utilities.scss
└── main.scss          # Archivo principal que importa todo
```

## Notas

- El archivo CSS compilado se genera en `css/style.css`
- El archivo `css/style.css` debe estar incluido en el repositorio
- Si modificas archivos SCSS, recuerda recompilar antes de commitear


