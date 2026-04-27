# oscarsoto.net — Web Personal

**Estado:** En producción  
**Última actualización:** 2026-04-27

## Objetivo

Web personal moderna y profesional en HTML estático, reemplazando la anterior en Google Sites.

## Stack

| Componente | Herramienta |
|---|---|
| Dominio | oscarsoto.net (DNS en Squarespace) |
| Hosting | GitHub Pages (rama `main`) |
| Repo | github.com/oscarsa85/oscarsoto.net |
| URL pública | https://oscarsoto.net |

## Archivos del proyecto

```
oscarsoto.net/
├── index.html            — Web completa (single-page, self-contained)
├── CNAME                 — Dominio personalizado para GitHub Pages
└── uploads/
    ├── portrait_v2.png   — Foto de perfil (about)
    ├── Sacha.jpeg        — Foto testimonial (Sacha B.)
    ├── Aleix.jpeg        — Foto testimonial (Aleix P.)
    └── Dani.jpeg         — Foto testimonial (Daniel A.)
```

## Estructura de la web (secciones)

1. **Hero** — nombre centrado, tagline, CTA
2. **About** — bio, foto de perfil reducida, tags
3. **Skills** — 6 áreas de expertise con certificaciones
4. **Work** — timeline de experiencia profesional (4 etapas)
5. **Testimonials** — 3 recomendaciones de LinkedIn con foto
6. **Blog** — 3 posts destacados de pmtricks.net
7. **Connect** — connect@oscarsoto.net + LinkedIn + pmtricks.net

## DNS (Squarespace) — registros relevantes

| Tipo | Nombre | Datos | Notas |
|------|--------|-------|-------|
| A | @ | 185.199.108-111.153 (×4) | GitHub Pages |
| CNAME | www | oscarsa85.github.io | GitHub Pages |
| A | n8n | 143.47.39.58 | **CRÍTICO — n8n producción** |
| MX | @ | mxa/mxb.mailgun.org | Correo activo |

## Decisiones tomadas

- Hero centrado, sin watermark "OS"
- Foto en sección About (320px, centrada, 40px margen superior)
- Email de contacto: connect@oscarsoto.net
- Redirección Squarespace `oscarsoto.net → www.oscarsoto.net` eliminada (innecesaria con GitHub Pages)
- `oscarsoto.html` eliminado — `index.html` es la única fuente

## Próximos pasos

- [ ] Activar "Enforce HTTPS" en GitHub Pages (esperar emisión de certificado SSL)
- [ ] Actualizar posts del blog cuando se relance pmtricks.net
