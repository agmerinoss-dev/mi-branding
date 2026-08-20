# 02 — Sistema visual

## Paleta

| Rol | Hex | Token | Uso | Proporción |
|---|---|---|---|---|
| Negro | `#0C1014` | `--vt-black` | Fondo de casi toda pieza | 80–85% |
| Gris oscuro | `#4C4C4C` | `--vt-gray` | Texto secundario, líneas, metadatos | 10–15% |
| Violeta | `#8B6FB0` | `--vt-violet` | Un acento puntual, glow | <5% |
| Blanco | `#FFFFFF` | `--vt-white` | Titulares y cuerpo sobre negro | según texto |

**Regla del violeta:** condimento, no plato principal. Máximo un elemento en
violeta por pieza — una palabra del titular, *o* un glow, *o* un punto indicador.
Nunca los tres. Nunca como fondo. Nunca un titular completo en violeta.

Escala derivada permitida (solo para opacidades, no colores nuevos):
`--vt-white-64`, `--vt-white-40`, `--vt-violet-glow` (radial, 12–18% de opacidad).

**Legibilidad sobre negro:** el gris `#4C4C4C` funciona para líneas, metadatos y etiquetas, pero se cae cuando lleva un párrafo entero. Para texto de apoyo sobre fondo negro se usa blanco al 64% (`--vt-white-64`). El gris se reserva para elementos secundarios cortos y para texto sobre fondo claro.

Prohibido: verde (es color de estado de la plataforma, no de marca), azul,
gradientes multicolor, cualquier hex fuera de esta tabla.

## Tipografía

| Rol | Fuente | Peso / estilo | Tracking |
|---|---|---|---|
| Titular | Geist | 400 regular — **nunca 600/700** | −0.02em |
| Wordmark VENTUREST | Geist | 400, mayúsculas, con ® pequeño | 0.04em |
| Eyebrow / etiqueta | IBM Plex Mono | 400/500, MAYÚSCULAS | 0.12em |
| Cuerpo | Geist | 400 | 0 |
| Acento cursivo | Instrument Sans | 300 italic — uso raro | 0 |

Lo que parece "grueso" en las piezas existentes es el trazo propio de Geist.
No forzar bold nunca. Si un titular necesita más presencia, se sube el tamaño
o se acorta el texto — no el peso.

Escala tipográfica para lienzo 1080px:
`display 96 / headline 72 / subhead 48 / body 32 / eyebrow 22 / caption 18`

Interlineado: 1.05 en display y headline, 1.4 en cuerpo.

## Elementos gráficos recurrentes

**Marco HUD.** Líneas finas de 1–2px en forma de L, blancas o al 40% de opacidad,
en una o dos esquinas. Nunca las cuatro: eso lo convierte en marco decorativo.
Largo del brazo: ~8% del ancho de la pieza.

**Glow violeta.** Radial difuso, anclado a un borde o esquina. Nunca detrás del
texto principal, nunca más de un cuarto del frame. Opacidad baja: se intuye, no se ve.

**Bloque de coordenadas.** IBM Plex Mono mayúsculas, gris o blanco al 64%:
`39°28'N 0°22'W · [VALENCIA] · OCTOBER`
Va en un borde, como metadato — no compite con el titular.

**Eyebrow con corchetes.** `[ED_01 DIGITAL TRENDS]`, `[PARTNER PROGRAM]`.
Los corchetes son parte del sistema, no adorno: señalan categoría.

**Textura grid / blueprint.** Cuadrícula fina al 4–6% de opacidad blanca.
Opcional, reservada a posters de evento. No en piezas de copy.

**Prensa como prueba.** Recorte o mención de medio insertado directo,
sin marco, sombra ni tarjeta. El recorte crudo es el punto.

## Fotografía

- Real, cruda, del equipo y de eventos. No stock, no posada, no apretones de mano.
- Sin filtros que suavicen. El contraste lo da el fondo negro, no la foto.
- Merchandising: camisetas negras con wordmark blanco.
- Cuando la foto va de fondo: overlay negro 45–65% para que el texto respire.

## Plantillas de composición

**Post statement (1080×1080 o 1080×1350)**
Fondo negro pleno → eyebrow mono arriba → titular Geist regular blanco alineado a
la izquierda → una línea de apoyo en gris → wordmark pequeño en esquina inferior →
glow violeta opcional en un extremo.

**Story CTA (1080×1920)**
Foto real de fondo con overlay → headline corto arriba → cuerpo en 2–3 líneas →
CTA en caja de alto contraste (negro sobre blanco o blanco sobre negro).
El CTA nunca en violeta pleno.

**Story de recurso (1080×1920)**
Captura de pantalla o documento como protagonista, ligeramente rotada o con marco
HUD → texto de contexto alrededor en Geist → etiqueta mono si aplica.

**Slide de carrusel (1080×1350)**
Un dato o una idea por slide. Numeración mono en esquina (`01 / 06`) solo si el
carrusel es realmente una secuencia. Último slide = CTA.

**Poster de evento (1080×1350)**
Grid blueprint de fondo → nombre del evento en display → bloque de coordenadas →
fecha en mono → wordmark.

## Márgenes y ritmo

- Margen de seguridad: 72px en lienzo de 1080 (6.6%).
- Story: además, 240px libres arriba y 320px abajo (zona de UI de Instagram).
- Un solo punto focal por pieza. Si hay dos titulares compitiendo, sobra uno.

## Checklist antes de exportar

- [ ] Fondo negro
- [ ] Violeta en máximo un elemento
- [ ] Geist sin bold
- [ ] Eyebrow en IBM Plex Mono mayúsculas
- [ ] Foto real, no stock
- [ ] Un dato concreto en el copy
- [ ] Sin exclamaciones ni jerga de infoproducto
- [ ] Wordmark presente y pequeño
