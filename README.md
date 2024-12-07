
# SCSS Starter Kit

A modular and scalable SCSS boilerplate for front-end projects. This structure is designed to organize your styles efficiently and maintain consistency across your projects.

---

## 📂 Folder Structure

```
scss/
├── abstracts/      # Variables, mixins, and functions
│   ├── _breakpoints.scss
│   ├── _colors.scss
│   ├── _font-constants.scss
│   ├── _font-face.scss
│   ├── _functions.scss
│   ├── _mixins.scss
│   └── _index.scss
├── base/           # Base styles (reset, typography, utilities)
│   ├── _base.scss
│   ├── _typography.scss
│   ├── _utilities.scss
│   └── _index.scss
├── components/     # Component-specific styles
│   ├── _buttons.scss
│   ├── _navbar.scss
│   └── _index.scss
├── layout/         # Layout styles (header, footer, sidebar)
│   ├── _header.scss
│   ├── _footer.scss
│   ├── _sidebar.scss
│   └── _index.scss
├── pages/          # Page-specific styles
│   └── _index.scss
├── themes/         # Theme-specific styles (light, dark, etc.)
│   ├── _light.scss
│   ├── _dark.scss
│   ├── _themes-mixins.scss
│   └── _index.scss
├── vendor/         # Third-party styles (e.g., Normalize.css)
│   └── _index.scss
└── style.scss      # Main entry point for all styles
```

---

## 🌟 Features

- **Modularity**: Organized into clear and reusable modules.
- **Scalability**: Easily add new components, pages, or themes.
- **Theming**: Includes mixins and variables for light and dark themes.
- **Responsive Design**: Includes predefined breakpoints for different devices.
- **Best Practices**: Follows SCSS architecture principles.

---

## 📜 Usage

### 1. Clone the repository
```bash
git clone https://github.com/your-username/scss-starter-kit.git
```

### 2. Import the SCSS entry point
Import `style.scss` into your project:
```scss
@import './scss/style.scss';
```

### 3. Customize
- Update the variables in `abstracts/_variables.scss` to match your project.
- Add or modify components, layouts, or themes as needed.

---

## 📋 Breakpoints

The following breakpoints are defined in `abstracts/_breakpoints.scss`:
```scss
$bp-xs: 575px;   // X-Small (phones)
$bp-sm: 576px;   // Small (phones)
$bp-md: 768px;   // Medium (tablets)
$bp-lg: 992px;   // Large (desktops)
$bp-xl: 1200px;  // Extra Large (desktops)
$bp-xxl: 1400px; // Extra Extra Large (desktops)
```

---

## 🎨 Themes

This boilerplate includes `light` and `dark` themes. To apply a theme:
1. Add the corresponding class to the `html` element (`light` or `dark`).
2. Use the defined mixins in `themes/_themes-mixins.scss` to customize styles.

```html
<html class="light">
  <head>
    <link rel="stylesheet" href="styles.css">
  </head>
  <body>
    <p>SCSS Starter Kit in action!</p>
  </body>
</html>
```

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).