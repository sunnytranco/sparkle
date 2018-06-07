---
description: >-
  Using system-ui in development but when we design, only SF Pro Text and SF Pro
  Display could be used due to consistency requirement and major diff from
  development
---

# Typography

## Font stacks

We use system-ui fonts to make sure that our user will have the best experience 'cause with this font stack the browser won't need to download fonts from other source, providing faster page load and better display compatible as a system fonts. 

{% hint style="info" %}
We use sans-serif fonts for most of our type, the exception being when you want to display code then you should defer to monospace fonts.
{% endhint %}

### San-serif

```css
font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', 'Roboto', 'Oxygen', 'Ubuntu', 'Fira Sans', 'Droid Sans', 'Helvetica Neue', sans-serif;
```

### Monospaced

```css
font-family: "SF Mono", "Segoe UI Mono", "Roboto Mono", "Ubuntu Mono", Menlo, Courier, monospace;
```

## Font colors

We have two color palettes for typography. Based on which element and state we use appropriate color to ensuring sufficient color contrast between elements so that people with low vision can see and use the interface.



