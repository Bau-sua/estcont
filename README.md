# Numeria — Landing Page para Estudios Contables

Landing page estática, minimalista y profesional para estudios contables. Construida con **Astro** y **Tailwind CSS**, deploy instantáneo en **Cloudflare Pages**.

[![Astro](https://img.shields.io/badge/Astro-5.0-BC52EE?logo=astro)](https://astro.build)
[![Tailwind](https://img.shields.io/badge/Tailwind-4.0-38BDF8?logo=tailwindcss)](https://tailwindcss.com)
[![Cloudflare Pages](https://img.shields.io/badge/Cloudflare-Pages-F38020?logo=cloudflare)](https://pages.cloudflare.com)

![Hero section preview — clean typography on cream background](https://raw.githubusercontent.com/Bau-sua/estcont/main/.github/preview.png)

## 🎯 Ideal para

- Estudios contables chicos y medianos
- Páginas one-page tipo "landing" para captar clientes
- Base para customizar por cliente (fork del repo)

## 📐 Estructura

```
Hero        → Headline, subtítulo, CTA doble
Servicios   → 3 cards (contable, impuestos, sueldos)
Ventajas    → 3 razones (digital, atención real, precio fijo)
Proceso     → 3 pasos (consultar → analizar → resolver)
Testimonios → 2 citas de clientes
Contacto    → Formulario + WhatsApp
Footer      → Email, teléfono, copyright
```

## 🎨 Diseño

- **Estilo:** minimalista, tipografía grande, mucho espacio en blanco
- **Paleta:** 5 colores (teal, lima, borravino, gris violáceo, crema)
- **Responsivo:** mobile-first con Tailwind breakpoints
- **Peso final:** ~12 KB de HTML + ~5 KB de CSS

## 🚀 Deploy en Cloudflare Pages

1. Conectá tu repo de GitHub en [Cloudflare Pages](https://dash.cloudflare.com/)
2. Build command: `npm run build`
3. Output directory: `dist`
4. Deploy automático en cada push a `main`

## ⚙️ Stack

| Capa      | Tecnología                    |
| --------- | ----------------------------- |
| Framework | Astro 5 (SSG, cero JS)        |
| Estilos   | Tailwind CSS 4                |
| Forms     | Formspree o Cloudflare Worker |
| Hosting   | Cloudflare Pages (free tier)  |
| Dominio   | Custom via Cloudflare DNS     |

## 🔁 Modelo de trabajo

Este repo es el template base. Para cada cliente nuevo:

```bash
# Cloná el repo
git clone git@github.com:Bau-sua/estcont.git cliente-nuevo

# O mejor, forkealo desde GitHub y clonalo
gh repo fork Bau-sua/estcont --clone
```

Y después customizá:

- Colores en `src/styles/global.css`
- Copy en cada componente
- WhatsApp y datos de contacto

## 📁 Estructura del proyecto

```
.
├── src/
│   ├── pages/index.astro          ← Página principal
│   ├── layouts/BaseLayout.astro   ← Layout HTML shell
│   ├── components/
│   │   ├── Hero.astro
│   │   ├── Servicios.astro
│   │   ├── Ventajas.astro
│   │   ├── Proceso.astro
│   │   ├── Testimonios.astro
│   │   ├── Contacto.astro
│   │   └── Footer.astro
│   └── styles/global.css          ← Paleta y config Tailwind
├── public/                        ← Assets estáticos
├── astro.config.mjs
├── package.json
└── dist/                          ← Build output (gitignored)
```

## 📝 Desarrollo local

```bash
npm install
npm run dev        # http://localhost:4321
npm run build      # output → dist/
```

---

**Template por [Bau-sua](https://github.com/Bau-sua)** · Licencia MIT
