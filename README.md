# POS gastronómico en la nube

![Next.js](https://img.shields.io/badge/Next.js-App%20Router-000000?logo=nextdotjs&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3FCF8E?logo=supabase&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind%20CSS-06B6D4?logo=tailwindcss&logoColor=white)
![shadcn/ui](https://img.shields.io/badge/shadcn%2Fui-000000)
![Estado](https://img.shields.io/badge/estado-en%20desarrollo-eda100)

> 🇬🇧 **English summary:** Cloud-native point-of-sale system for restaurants built with Next.js (App Router), Supabase, Tailwind CSS and shadcn/ui: visual table layout, end-of-shift cash closing, drag-and-drop floor editor for admins, and role-based login (admin by email, waiters by PIN).

<!-- 📸 Agregá acá una captura o un GIF del módulo de salón: es lo primero que mira un reclutador. -->
<!-- ![Gestión de salón](docs/salon.png) -->

## El problema

<!-- Contá con tus palabras qué problema viste en los POS que usaste como supervisor de operaciones. -->
Trabajé años en operaciones gastronómicas. Este proyecto es un punto de venta que corre en el navegador, pensado para cómo se trabaja de verdad en un salón: el plano real del local, mozos que necesitan entrar rápido y un cierre de caja simple.

## Módulos

| Módulo | Qué hace | Estado |
|---|---|---|
| **Gestión de salón** | Grilla visual con las mesas del local | 🚧 En desarrollo |
| **Cierre de caja** | Cierre del turno | Planificado |
| **Administración** | Editor del plano con arrastrar y soltar: cada mesa en su posición real | Planificado |
| **Login y roles** | Administrador con email; mozos con PIN para entrar rápido desde la tablet | Planificado |

## Decisiones de diseño

- **El plano se dibuja como es el local.** El administrador ubica las mesas arrastrándolas; el mozo ve exactamente lo que tiene adelante.
- **Dos formas de entrar.** El administrador usa email y contraseña. Los mozos usan un PIN corto, porque en pleno servicio nadie escribe un email.
- **Todo en la nube, costo cero para empezar.** Next.js en Vercel y Supabase en su plan gratuito.

## Stack

- **Frontend:** Next.js (App Router), Tailwind CSS, shadcn/ui
- **Backend y base de datos:** Supabase (PostgreSQL, autenticación, tiempo real)
- **Deploy:** Vercel

## Cómo ejecutarlo

```bash
git clone https://github.com/Lu1sPerez/pos-gastronomico.git
cd pos-gastronomico
npm install
cp .env.example .env.local   # completar NEXT_PUBLIC_SUPABASE_URL y NEXT_PUBLIC_SUPABASE_ANON_KEY
npm run dev
```

## Próximos pasos

- [ ] Terminar gestión de salón
- [ ] Cierre de caja
- [ ] Editor de plano para administradores
- [ ] Login con roles
- [ ] Deploy en Vercel con demo pública

---
**Autor:** Luis Pérez · [LinkedIn](https://www.linkedin.com/in/perezluis24/) · Analista de Datos | BI | Automatización
