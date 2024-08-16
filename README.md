# css-tricks

## CSS Reset June 2024

```css
/* CSS RESET June 2024 */

* { margin: 0; padding: 0; }
*, *::before, *::after { box-sizing: border-box; }

body { min-height: 100dvh; }
input, button, textarea, select { font: inherit; }

p { text-wrap: pretty; }
h1, h2, h3, h4, h5, h6 { text-wrap: balance; }

img, video, svg { height: auto; max-width: 100%; }

@media (prefers-reduced-motion: reduce) {
	table {
		width: 100%;
	}
}

@media (max-width: 768px) {
	*, *::before, *::after {
		animation-duration: 0.01ms !important;
		animation-iteration-count: 1 !important;
		transition-duration: 0.01ms !important;
		scroll-behavior: auto !important;
		transition: none;
	}
}
```

## CSS para que automáticamente se puedan alinear imágenes en un grid y que sea responsive:

1. Image in grid

```css
div > img {
  border-radius: 8px;
  width: 100%;
  height: auto;
  box-shadow: 0 0 30px #0000;
}
div {
  display: grid;
  grid-template-columns: repeat(auto-fit; min-max(150px, 1fr));
  gap: 32 px;
}
```

2. Image in flex

```css
  display: flex;
  align-items: center;
  flex-direction: row;
  justify-content: center;
  gap: 2rem;
```

## Varias formas de centrar un elemento verticalmente. [Fuente midu.dev](https://midu.dev/centrar-elementos-css/)

```css
.container {
  display: flex;
  justify-content: center;
  align-items: center;
}
```

[Demo](https://codi.link/PGRpdiBjbGFzcz0nY29udGFpbmVyJz4KICA8aDE+VGV4dG8gY2VudHJhZG88L2gxPgo8L2Rpdj4=%7CLmNvbnRhaW5lciB7CiAgZGlzcGxheTogZmxleDsKICBqdXN0aWZ5LWNvbnRlbnQ6IGNlbnRlcjsKICBhbGlnbi1pdGVtczogY2VudGVyOwp9CgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCmJvZHkgewogIGJhY2tncm91bmQ6ICMwOWY7CiAgZm9udC1mYW1pbHk6IHN5c3RlbS11aTsKfQoKaDEgewogIGJhY2tncm91bmQ6ICNmZmY7CiAgcGFkZGluZzogMTZweDsKfQoKLmNvbnRhaW5lciB7CiAgaGVpZ2h0OiA5NnZoOwp9%7C)



