---
version: alpha
name: jonmircha
description: Sistema de diseno moderno, energetico y docente — naranja accesible como accion principal, minimalista y de alto contraste.
colors:
  primary: "#C7431F"
  primary-alt: "#E7562E"
  primary-variant: "#E7762E"
  primary-hover: "#A93A14"
  primary-pressed: "#9C3612"
  link: "#0088CC"
  ink: "#202225"
  muted: "#808080"
  surface: "#FCFCFC"
  surface-muted: "#EEEEEE"
  disabled: "#CCCCCC"
  white: "#FFFFFF"
typography:
  display:
    fontFamily: "Raleway Black"
    fontSize: 40px
    fontWeight: 900
    lineHeight: 48px
  h1:
    fontFamily: "PT Sans"
    fontSize: 40px
    fontWeight: 700
    lineHeight: 48px # REVIEW: interlineado no especificado en origen, asumido igual que display
  h2:
    fontFamily: "Raleway Black"
    fontSize: 40px
    fontWeight: 900
    lineHeight: 48px # REVIEW: interlineado no especificado, asumido 48px
  h3:
    fontFamily: "PT Sans"
    fontSize: 16px
    fontWeight: 700
    lineHeight: 24px # REVIEW: interlineado no especificado, asumido 24px
  body:
    fontFamily: "PT Sans"
    fontSize: 20px
    fontWeight: 400 # REVIEW: peso no especificado, asumido 400
    lineHeight: 30px
  list-item:
    fontFamily: "Raleway"
    fontSize: 20px
    fontWeight: 400 # REVIEW: peso no especificado, asumido 400
    lineHeight: 30px # REVIEW: interlineado no especificado, asumido igual que body
  small:
    fontFamily: "Raleway"
    fontSize: 16px
    fontWeight: 400 # REVIEW: peso e interlineado no especificados, asumido 400 / 24px
    lineHeight: 24px # REVIEW: valor asumido
  button-label:
    fontFamily: "Raleway"
    fontSize: 19.216px
    fontWeight: 700 # REVIEW: peso no especificado, asumido 700
    lineHeight: 24px # REVIEW: interlineado no especificado, asumido 24px
  link:
    fontFamily: "PT Sans"
    fontSize: 20px
    fontWeight: 400 # REVIEW: peso no especificado, asumido 400
    lineHeight: 30px # REVIEW: interlineado no especificado, asumido igual que body
  label:
    fontFamily: "PT Sans"
    fontSize: 16px
    fontWeight: 700
    lineHeight: 24px # REVIEW: interlineado no especificado, asumido 24px
  mono:
    fontFamily: "Roboto Mono"
    fontSize: 14px # REVIEW: tamano no especificado para fechas monoespaciadas, asumido 14px
    fontWeight: 400 # REVIEW: valor asumido
    lineHeight: 20px # REVIEW: valor asumido
  chip:
    fontFamily: "Raleway"
    fontSize: 13px # REVIEW: familia no especificada para chips, asumida Raleway
    fontWeight: 400 # REVIEW: valor asumido
    lineHeight: 16px # REVIEW: valor asumido
rounded:
  none: 0px
  sm: 8px
  md: 16px
  pill: 50px
  full: 9999px # REVIEW: origen dice 50% para circulos; se mapea a 9999px por compatibilidad con spec (Dimension solo admite px/em/rem)
spacing:
  base: 8px
  micro: 4px
  xs: 8px
  sm: 12px
  md: 16px
  lg: 24px
  xl: 32px
  2xl: 40px # REVIEW: valor interpolado, no estaba en la escala original
  3xl: 48px
  4xl: 92px
  5xl: 136px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.white}"
    typography: "{typography.button-label}"
    rounded: "{rounded.pill}"
    padding: 12px # REVIEW: origen dice 12px x 24px; se registra un solo valor, ver paddingX/paddingY en prosa
  button-primary-hover:
    backgroundColor: "{colors.primary-hover}"
    textColor: "{colors.white}"
  button-primary-pressed:
    backgroundColor: "{colors.primary-pressed}"
    textColor: "{colors.white}"
  button-primary-disabled:
    backgroundColor: "{colors.disabled}"
    textColor: "{colors.muted}"
  button-icon:
    backgroundColor: "{colors.surface-muted}"
    textColor: "{colors.primary}"
    rounded: "{rounded.full}"
    size: 32px
  button-icon-hover:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.white}"
  button-ghost:
    backgroundColor: "transparent"
    textColor: "{colors.link}"
    typography: "{typography.link}"
  button-ghost-hover:
    backgroundColor: "transparent"
    textColor: "{colors.primary}"
  card:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.ink}"
    typography: "{typography.body}"
    rounded: "{rounded.none}"
    padding: 12px # REVIEW: origen dice 12-24px; se registra base 12px
  navbar:
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
    height: 64px
  input:
    backgroundColor: "{colors.white}"
    textColor: "{colors.ink}"
    typography: "{typography.body}"
    rounded: "{rounded.none}"
    padding: 12px # REVIEW: origen dice 12px x 16px; se registra base
  input-focus:
    backgroundColor: "{colors.white}"
    textColor: "{colors.ink}"
  social-icon:
    backgroundColor: "{colors.surface-muted}"
    textColor: "{colors.ink}"
    rounded: "{rounded.full}"
    size: 32px
  social-icon-hover:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.white}"
  chip:
    backgroundColor: "{colors.surface-muted}"
    textColor: "{colors.ink}"
    typography: "{typography.chip}"
    rounded: "{rounded.full}"
  avatar:
    rounded: "{rounded.full}"
    size: 200px
  contact-button:
    backgroundColor: "{colors.white}"
    textColor: "{colors.ink}"
    rounded: "{rounded.none}"
  contact-button-hover:
    backgroundColor: "{colors.white}"
    textColor: "{colors.primary}"
  course-card:
    backgroundColor: "{colors.white}"
    textColor: "{colors.ink}"
    rounded: "{rounded.none}"
  course-card-hover:
    backgroundColor: "{colors.white}"
    textColor: "{colors.ink}"
  edu-card:
    backgroundColor: "{colors.white}"
    textColor: "{colors.ink}"
    rounded: "{rounded.none}"
---

# jonmircha — DESIGN.md

## Overview

Estetica moderna, energetica y centrada en la docencia: puente entre experiencia tecnica y calidez cercana. Naranja accesible ({colors.primary}) como accion principal, con el naranja de marca ({colors.primary-alt}) reservado a uso alternativo/decorativo, sobre fondos casi blancos ({colors.surface}, {colors.white}).

Filosofia minimalista: layouts limpios, mucho espacio en blanco, tipografia con proposito y componentes sin ornamentacion innecesaria. Publico: creadores y desarrolladores; respeta el tiempo y la carga cognitiva. En una frase: acento audaz sin abrumar, alto contraste y jerarquia por tamano, peso y color — nunca por opacidad.

Motivo de marca: logo del buho construido con degradado naranja de {colors.primary-alt} a {colors.primary-variant}.

> **REVIEW:** degradado exacto del logo (paradas de color y angulo) no especificado en origen; definir stops si se va a usar en codigo.

## Colors

Paleta de alto contraste: naranja accesible como principal + naranja de marca alternativo + azul funcional + neutros claros.

- **Primary / Naranja accesible ({colors.primary} #C7431F):** CTA primarios, acentos y texto/botones en blanco. Contraste 4.94:1 sobre blanco.
- **Primary alt / Naranja de marca ({colors.primary-alt} #E7562E):** uso alternativo/decorativo y titulares grandes; no usar para texto pequeno en blanco (3.64:1).
- **Primary variant / Naranja alterno ({colors.primary-variant} #E7762E):** enfasis puntual, variante sutil del naranja.
- **Primary hover ({colors.primary-hover} #A93A14):** estado hover del boton primario. **REVIEW:** oscurecido desde el #D94D1F original para mantener progresion accesible sobre el nuevo primary.
- **Primary pressed ({colors.primary-pressed} #9C3612):** estado pressed del boton primario. **REVIEW:** oscurecido para ser el tono mas profundo de la escala.
- **Link / Azul cielo ({colors.link} #0088CC):** enlaces en texto y elementos interactivos secundarios.
- **Ink / Negro casi puro ({colors.ink} #202225):** texto principal, maximo contraste sobre claro.
- **Muted / Gris medio ({colors.muted} #808080):** texto terciario y deshabilitados. No usar grises mas claros que este para texto.
- **Surface ({colors.surface} #FCFCFC):** fondo base, casi blanco.
- **Surface muted ({colors.surface-muted} #EEEEEE):** fondo de botones secundarios/fantasma, bordes y chips.
- **Disabled ({colors.disabled} #CCCCCC):** fondo de boton primario deshabilitado.
- **White ({colors.white} #FFFFFF):** maximo contraste, fondos de campos y tarjetas.

Colores descartados por falta de uso (linter `orphaned-tokens`): cian claro #73CFFA, carbones #2B3A42/#20252C/#202B38 y fondo alternativo #F7F7F7.

Regla: combinar {colors.primary} con {colors.white} y {colors.surface-muted} para maximo contraste. No mezclar naranja y azul en el mismo elemento interactivo; elegir uno.

## Typography

Tres familias con roles claros. Fuentes via Google Fonts — **REVIEW:** pesos exactos a cargar no especificados; se asume PT Sans 400+700, Raleway 400+700+900, Roboto Mono 400.

- **Display ({typography.display}):** Raleway Black 40px / 48px. Solo titulares mas importantes, uso moderado.
- **H1 ({typography.h1}):** PT Sans 40px peso 700. **REVIEW:** line-height asumido 48px.
- **H2 ({typography.h2}):** Raleway Black 40px. **REVIEW:** line-height asumido 48px.
- **H3 ({typography.h3}):** PT Sans 16px peso 700 para subsecciones. **REVIEW:** line-height asumido 24px.
- **Body ({typography.body}):** PT Sans 20px / 30px. Base 20px en escritorio, nunca bajo 16px; en movil 18–20px.
- **List item ({typography.list-item}):** Raleway 20px.
- **Small ({typography.small}):** Raleway 16px.
- **Button label ({typography.button-label}):** Raleway 19.216px, asumido peso 700. **REVIEW:** confirmar peso y si 19.216px debe redondearse a 19px.
- **Link ({typography.link}):** PT Sans 20px.
- **Label ({typography.label}):** PT Sans 16px peso 700 para etiquetas de formulario.
- **Mono ({typography.mono}):** Roboto Mono para codigo y fechas en tarjetas edu/experiencia. **REVIEW:** tamano asumido 14px.
- **Chip ({typography.chip}):** 13px tipo pildora. **REVIEW:** familia asumida Raleway.

Jerarquia solo con tamano, peso y color, nunca con opacidad. No usar serif en la jerarquia principal. Titulares en movil pueden bajar pero nunca de 24px.

> **REVIEW:** `letterSpacing` no especificado en origen; se omite (equivalente a normal). Definir si se requiere tracking especifico.

## Layout

Modelo: mobile-first, 4 breakpoints, reticula de columnas con max-width centrado.

- **Base de espaciado:** {spacing.base} (8px). Escala: {spacing.micro} 4px micro, {spacing.xs} 8px, {spacing.sm} 12px, {spacing.md} 16px, {spacing.lg} 24px, {spacing.xl} 32px, {spacing.2xl} 40px (interpolado, REVIEW), {spacing.3xl} 48px, {spacing.4xl} 92px, {spacing.5xl} 136px.
- **Internos:** botones y campos 12–16px; tarjetas 12–24px; hero 48px horizontal / 92px vertical.
- **Secciones:** separacion vertical 48–92px (minimo 92px para zonas visuales claras en escritorio); en movil 24px, tableta 48px, escritorio 92px, amplio 92–136px.
- **Ancho maximo:** 1440px centrado.
- **Reticulas:** escritorio 12 columnas; tableta 8 columnas con margenes 48px; movil 1 columna con margenes 12–16px (12px base).
- **Breakpoints:** movil 320–599px (1 col), tableta 600–1023px (2–3 col), escritorio 1024–1439px (3+ col), amplio 1440px+ (max-width centrado).
- **Tactil:** interactivos minimo 44x44px; campos minimo 40px de alto. En movil la navegacion se apila o colapsa a hamburguesa; tarjetas a 1 columna.

> **REVIEW:** hay tension entre boton-icono de 32px definido en Componentes y minimo tactil de 44px; se conserva 32px visual con area tactil 44px recomendada. Gutter de reticula no especificado; asumir 24px.

## Elevation & Depth

Diseno mayormente plano. Sombras suaves y difusas solo con interaccion o apilamiento. Nunca mas profundas que `0 8px 24px`.

- **Plano (sin sombra):** tarjetas en reposo, campos, navegacion.
- **Sutil `0 2px 4px`:** hover de tarjetas.
- **Media `0 4px 12px`:** tarjetas elevadas, modales, popovers.
- **Alta `0 8px 24px`:** botones flotantes.
- **Velo de modal:** negro al 0.5 sobre el contenido.

> **REVIEW:** color de sombra no especificado; asumir `rgba(32,34,37,0.08/0.12/0.16)` derivado de {colors.ink} con opacidades 0.08 / 0.12 / 0.16 respectivamente. Velo asumido `rgba(0,0,0,0.5)`. Sin tokens `elevation` en front matter por limite del schema oficial (solo colors/typography/spacing/rounded/components); estos valores viven aqui en prosa.

## Shapes

Lenguaje nitido y moderno: recto por defecto.

- **None ({rounded.none} 0px):** defecto en tarjetas, campos, botones de contacto, course-cards y edu-cards.
- **SM ({rounded.sm} 8px):** opcional en elementos flotantes.
- **MD ({rounded.md} 16px):** reservado para componentes especiales.
- **Pill ({rounded.pill} 50px):** boton primario tipo pildora.
- **Full ({rounded.full} 9999px = 50%):** iconos, avatar, chips y badges circulares. **REVIEW:** mapeado de 50% a 9999px por schema.

No mezclar esquinas redondeadas y rectas en la misma vista.

## Components

### Botones

- **Primario ({components.button-primary}):** fondo {colors.primary}, texto {colors.white}, {typography.button-label}, pildora {rounded.pill}, padding 12px vertical / 24px horizontal. Hover a {components.button-primary-hover} ({colors.primary-hover}); pressed a {components.button-primary-pressed} ({colors.primary-pressed}) con encogido ligero; deshabilitado en {components.button-primary-disabled} (fondo {colors.disabled}, texto {colors.muted}). Altura minima 40px rectangular.
- **Secundario / icono circular ({components.button-icon}):** 32x32px, fondo {colors.surface-muted}, icono {colors.primary}, {rounded.full}. Hover invierte a {components.button-icon-hover} (fondo {colors.primary}, icono {colors.white}).
- **Fantasma ({components.button-ghost}):** sin fondo, texto {colors.link} en {typography.link}. Hover ({components.button-ghost-hover}): texto {colors.primary} con subrayado.

### Tarjetas y contenedores

- **Tarjeta de contenido ({components.card}):** fondo transparente o {colors.surface}, texto {colors.ink} en {typography.body}, {rounded.none}, padding horizontal 12px (rango 12–24px). Hover: sombra sutil.
- **Hero:** ancho completo, fondo {colors.white} o {colors.surface}, padding 48px horizontal / 92px vertical, max 1440px.
- **Navbar ({components.navbar}):** transparente, texto {colors.ink}, 64px alto, borde inferior opcional 1px {colors.surface-muted}.

### Campos y formularios

- **Input ({components.input}):** fondo {colors.white}, texto {colors.ink} en {typography.body}, padding 12px/16px, borde 2px {colors.surface-muted}, {rounded.none}. Focus ({components.input-focus}): borde {colors.primary} + halo suave {colors.primary} al ~20%. Placeholder {colors.muted}. Label en {typography.label}. **REVIEW:** opacidad/color exacto del halo no especificado; asumir `color-mix(in srgb, {colors.primary} 20%, transparent)`.

### Navegacion y enlaces

- **Menu:** PT Sans 20px {colors.ink}; hover {colors.primary} + subrayado 2px; activo subrayado 3px.
- **Enlace en texto:** {colors.link} sin subrayado; hover {colors.primary} con subrayado.
- **Enlace-titulo (Raleway Black):** {colors.primary}; hover opacidad 0.8.

### Iconos sociales ({components.social-icon})

Circulares 32x32px, fondo {colors.surface-muted}, icono {colors.ink} ({colors.primary} en variante secundaria). Hover ({components.social-icon-hover}): fondo {colors.primary}, icono {colors.white}.

### Etiquetas, avatar y tarjetas de contenido

- **Chip ({components.chip}):** pildora {rounded.full}, fondo {colors.surface-muted}, texto {colors.ink}, {typography.chip} 13px.
- **Avatar ({components.avatar}):** circulo {rounded.full}, 200px (160px movil), borde 4px gris claro. **REVIEW:** color de borde asumido {colors.surface-muted}.
- **Contacto ({components.contact-button}):** fondo {colors.white}, texto {colors.ink}, icono {colors.primary}, borde 1px gris, {rounded.none}. Hover: borde y texto {colors.primary}.
- **Curso (columna):** icono arriba, titulo Raleway 700 19px, enlace "Ver →" azul; fondo {colors.white}, borde gris, {rounded.none}; hover borde {colors.primary} + sombra sutil.
- **Habilidad:** icono acento {colors.primary} + texto, en tarjeta blanca con borde gris.
- **Educacion/experiencia ({components.edu-card}):** acento lateral izquierdo 4px {colors.primary}, fondo {colors.white}, borde gris, {rounded.none}; fila superior titulo/rol + fecha derecha en {typography.mono} gris {colors.muted}, seguida de descripcion.

## Do's and Don'ts

Do:

- Do usar {colors.primary} para todos los CTA primarios y enfasis de marca.
- Do mantener 20px como base de cuerpo en escritorio; nunca bajar de 16px.
- Do aplicar 48–92px vertical ({spacing.3xl}–{spacing.4xl}) entre secciones mayores.
- Do usar PT Sans para cuerpo/navegacion y Raleway Black solo para titulares top.
- Do combinar naranja con blancos y gris claro para maximo contraste.
- Do usar botones de icono circulares ({rounded.full}) para sociales y acciones secundarias.
- Do mantener tarjetas y componentes en {rounded.none} para apariencia nitida.
- Do implementar hover con cambio de color o subrayado, nunca solo con opacidad (excepcion: enlace-titulo que baja a 0.8).

Don't:

- Don't usar naranja y azul juntos en el mismo interactivo; elegir uno.
- Don't usar sombras mas profundas que `0 8px 24px`.
- Don't usar grises mas claros que {colors.muted} (#808080) para texto.
- Don't aplicar serif en la jerarquia principal.
- Don't hacer botones menores a 32px circulares o 40px de alto rectangulares (y respetar 44px tactil).
- Don't esconder navegacion critica tras dropdowns en movil sin necesidad.
- Don't usar fondos con imagen/textura que compitan con legibilidad.
