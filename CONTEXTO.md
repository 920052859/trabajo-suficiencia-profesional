# Contexto del proyecto — Página FIM-UNI Trabajo de Suficiencia Profesional

Repositorio: https://github.com/920052859/trabajo-suficiencia-profesional
Página publicada (GitHub Pages): https://920052859.github.io/trabajo-suficiencia-profesional/
Archivo principal: `index.html` (una sola página, sin build step, GSAP + ScrollTrigger vía CDN)

## Origen

Basado en el documento "Estructura del Trabajo de Suficiencia Profesional" (Dr. Aurelio Marcelo Padilla Ríos, UNI-FIM, Set. 2025) y en el material del curso ubicado en:
`D:\2026\07. SISTEMAS, IA Y AUTOMATIZACIÓN\Enseñar UNI`

## Autora

- Nombre: Corina Lazo (Corina Fanny Lazo Arroyo en documentos formales)
- Email: lazocorinafanny123@gmail.com
- LinkedIn: **pendiente** — la sección "Sobre la autora" tiene un botón de LinkedIn con URL placeholder (`https://www.linkedin.com/`). Falta que la usuaria comparta su URL real y confirme la frase de bio.

## Estructura de la página (secciones, en orden)

1. **Header fijo** con navegación (Inicio, Estructura, Proceso, Formato APA, Fuentes, Recursos) que resalta la sección activa al hacer scroll, más un indicador SVG de tornillo/perno hexagonal que gira según el progreso de scroll.
2. **Fondo animado (`#bgLayer`)**: capa fija con parallax, incluye:
   - Engranajes y pernos genéricos.
   - Vectorización del monumento icónico de la FIM-UNI (foto de referencia): turbina Pelton (generada dinámicamente con 12 álabes vía JS), volante de 6 radios, y el numeral "1".
   - Cuadrícula tipo plano técnico (blueprint grid) muy sutil.
3. **Cursor personalizado**: engranaje que sigue el mouse con inercia suave y gira continuamente; cambia a una bandera de meta al pasar sobre enlaces/botones (simboliza "ejecutar y finalizar la tesis"). Se desactiva en dispositivos táctiles.
4. **Hero**: título animado letra por letra, engranaje flotante que reacciona al scroll.
5. **Estructura General** (`#overview`): tarjetas de Capítulo I–IV.
6. **Proceso** (`#pinned`): sección pineada con scroll-scrubbed steps (Generalidades → Marco Teórico → Desarrollo → Resultados → Conclusiones).
7. **Formato APA** (`#format`): tarjetas de márgenes, tipografía, interlineado, papel (basado en especificaciones APA 7 del PDF original).
8. **Fuentes** (`#fuentes`): buscadores/bases de datos internacionales (Google Scholar, Scopus, Web of Science, IEEE Xplore, ScienceDirect, SpringerLink, MDPI, arXiv, ResearchGate, SciELO) y repositorios peruanos (ALICIA-Concytec, RENATI-Sunedu, Cybertesis UNI, Repositorio PUCP, Cybertesis UNMSM, Concytec).
9. **Recursos del Curso** (`#recursos`): sistema de pestañas General / Sesión 1 / Sesión 2 / Sesión 3 / Sesión 4 / Sesión 5, con transición animada GSAP. Sesiones 4 y 5 muestran placeholder "Próximamente" (no había material en la carpeta fuente).
10. **CTA** (`#cta`): "2026 · Lima – Perú" (corregido de 2025 a 2026).
11. **Sobre la autora** (`#autora`): bio corta + botón LinkedIn (pendiente URL real).
12. **Footer**: crédito discreto "© Corina Lazo · Recursos para la comunidad FIM-UNI" (se eliminó la línea "Página generada con GSAP...").

## Archivos descargables (`recursos/`)

Copiados y renombrados desde la carpeta fuente, **excluyendo** automatizaciones propias (labs, prompts, notebooks propios, blueprints, scripts) y archivos con datos personales de terceros (actas con nombres de estudiantes, capturas de Gmail, QR personal, listas de asesoría).

- `recursos/general/` — sílabos, programa TSP, guías, libros de metodología (Baena 2017, Tesis Fácil), MT616 IA.
- `recursos/sesion1/` — PPT, guía docente, laboratorio, plantillas (acta de constitución, plantilla APA), artículo Dialnet.
- `recursos/sesion2/` — PPT, guía docente, laboratorio.
- `recursos/sesion3/` — PPT.

Tamaño total aprox. 47MB (dentro de límites de GitHub).

## Enlaces externos publicados (por decisión explícita de la usuaria)

- **Grabaciones Webex de Sesión 1** (2 partes), publicadas **con contraseña visible** en la página — la usuaria confirmó explícitamente que quería publicar todo, incluida la contraseña, entendiendo que esto hace la grabación efectivamente pública para cualquiera con el enlace de la página.
- **Google Forms** de la actividad de Sesión 2.
- **Google Colab notebook** de Sesión 3.

## Decisiones y feedback relevantes

- Los archivos se suben como **descargables + resumen navegable** (no solo texto, no solo archivos crudos) — decisión explícita de la usuaria.
- Se excluyen deliberadamente "automatizaciones" propias de la usuaria (carpeta `U1_Agente_Investigacion_Labs` con prompts, notebooks, blueprints) del contenido público.
- El `min-height:100vh` original de cada sección causaba demasiado espacio en blanco; se cambió a padding compacto (`3.5rem`) con el hero como única excepción (`90vh`).
- Recordar que las páginas grandes (`git push` de ~47MB) pueden exceder el timeout por defecto de 2 minutos — usar `run_in_background` con timeout extendido.

## Pendientes

- [ ] URL real de LinkedIn de Corina Lazo y confirmación/ajuste de la frase de bio en `#autora`.
- [ ] Material de Sesión 4 y Sesión 5 (actualmente placeholder "Próximamente").
- [ ] Confirmar si se desea agregar grabaciones Webex de sesiones 2 y 3 (la usuaria indicó que solo tiene la de la sesión 1).
