# Pareto — Sitio web

Sitio estático de **Pareto** (marca de ICB Spain Investment SL): estudio de desarrollo de producto digital (dev + IA).

## Stack
HTML estático + CSS compartido. **Sin build step**: se despliega tal cual (Cloudflare Pages, GitHub Pages, Netlify…). Portable a Astro más adelante.

## Estructura
```
/                         Home (capa marca)
/desarrollo-de-apps/      Landing captación (CRO) — apps a medida
/software-a-medida/       Landing captación
/desarrollo-web-a-medida/ Landing captación
/especialista-prestashop/ Landing captación
/desarrollo-ecommerce/    Landing captación
/integraciones/           Landing captación (nuestro fuerte)
/ia-para-empresas/        Landing captación
/automatizacion-de-procesos/ Landing captación
/google-ads/              Landing captación (servicio de margen)
/proyectos/               Índice de portfolio + casos detalle (/proyectos/<slug>/)
/estudio/                 Sobre nosotros
/contacto/                Contacto
/aviso-legal/ /privacidad/ /cookies/   Legales (plantilla, pendiente revisión legal)
/assets/styles.css        Hoja de estilos compartida
/assets/logo-sprite.svg   Logo oficial (sprite, recoloreable por currentColor)
```

## Diseño
- **Estilo:** referencia Senda Momentum (geometría de línea, hover sutil, mono retro).
- **Colores marca:** verde racing `#004225` + acento lima `#c3fa95` sobre blanco cálido `#f5f4ef`.
- **Tipografía:** Poppins (display/cuerpo) + Fraunces *itálica* (acento) + Space Mono (datos).
- Sistema completo documentado fuera de este repo, en `propios/pareto/web/03-sistema-de-diseno.md`.

## Desarrollo local
```bash
python3 -m http.server 8799    # y abrir http://localhost:8799/
```
Las rutas son root-relative, por lo que requieren servirse (no abrir con `file://`).

## Pendiente
- Conectar el formulario de las landings a un endpoint real (Formspree/handler) + evento de conversión en GTM.
- Imagen pintada (óleo) para la escena del CTA de la Home (hoy placeholder geométrico).
- Datos legales reales (NIF, domicilio) en las páginas legales.
- **Contenidos en borrador, pendientes de revisión.**
