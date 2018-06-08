# Developer

Sparkle Design System provides front-end developers & engineers a collection of reusable HTML and SCSS partials to build websites and user interfaces. Adopting the library enables developers to use consistent markup, styles, and behavior in prototype and production work.

## Structure

```text
sparkle-ds/
|--components
|  |--button
|  |  |--button.vue
|  |  |--button.js
|  |  |--_button.scss
|  |  |--_mixins.scss
|--global
|  |--assets
|  |  |--images
|  |--fonts
|  |  |--sf-pro-text.woff
|  |--grid
|  |  |--_variables.scss
|  |  |--_grid.scss
|  |--scss
|  |  |--_colors.scss
|  |  |--_css--body.scss
|  |  |--_css--font-face.scss
|  |  |--_css--helpers.scss
|  |  |--_css--reset.scss
|  |  |--_css--typography.scss
|  |  |--_layer.scss
|  |  |--_layout.scss
|  |  |--_mixins.scss
|  |  |--_spacing.scss
|  |  |--_typography.scss
|  |  |--_vars.scss
|  |  |--style.scss
```

## SCSS

Using the Carbon Sass files infers usage of the SCSS pre-processor. All Sass files use the `*.scss` file extension.

If you're starting a new project without a boilerplate, you need to know about a few things to get started.

### **Autoprefixer**

Make sure your build process uses [autoprefixer](https://github.com/postcss/autoprefixer) to ensure vendor prefixes are automatically added to your output CSS.

### **Default body styles**

CSS is automatically applied to `<body>` element, which comes from [\_css--body.scss](https://github.com/carbon-design-system/carbon-components/blob/master/src/globals/scss/_css--body.scss). These styles are meant to cascade down to everything in `<body>` to set common styles shared across all components.

```css
body {
  @include reset;
  font-family: 'ibm-plex-sans';
  color: $text-01;
  background-color: $ui-02;
  line-height: 1;
}
```

### **Global SCSS variables**

These variables are used to configure which parts of the SCSS get compiled, where each variable controls a SCSS file of the same name. All variables are set to `true`by default, except for `_css--font-face.scss`

For example:

* When you set `$css--reset: true`, then the contents of [\_css--reset.scss](https://github.com/carbon-design-system/carbon-components/blob/master/src/globals/scss/_css--reset.scss) will be part of your output CSS.
* When you set `$css--reset: false`, then nothing gets included from that SCSS file.
* When the variable is not declared at all, then nothing gets included from that SCSS file.

The same rules apply to all the following variables:

```css
// In styles.scss:
// These are the default settings.
$css--font-face: false !default;
$css--helpers: true !default;
$css--body: true !default;
$css--use-layer: true !default;
$css--reset: true !default;
$css--typography: true !default;
$css--plex: true !default;
```

These flags are set for you by default when you `@import` the `styles.scss` file. You can override these default settings by redeclaring the variables.

### **Importing SCSS files**

To add a component style to your build, simply import the component directly.

```javascript
@import 'node_modules/sparkle-ds/components/button/button';
```

Importing a component this way will bring in any dependencies that component has as well. The import system removes duplicate dependencies, so shared dependencies between components will not create extra CSS.

### **Namespacing**

Carbon Components are built to be included individually and not clobber global styles - all `class` attributes are prefixed by the `nsds--` moniker. You can specify your own prefix by changing the SCSS variable `$prefix`.



