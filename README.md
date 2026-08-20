# Venturest — Contexto de marca para generación de diseño

Paquete de contexto para que un generador de diseño produzca piezas de Venturest
(principalmente Instagram: feed, stories, carruseles, posters de evento) sin tener
que preguntar por marca, tono o formato en cada iteración.

## Orden de lectura

| Archivo | Para qué sirve |
|---|---|
| `brand/01-brand-brief.md` | Qué es Venturest, a quién le habla, qué campaña está viva. Contexto de negocio. |
| `brand/02-visual-system.md` | Reglas visuales duras: paleta, tipografía, elementos, composición. |
| `brand/03-voice-and-copy.md` | Tono, estructuras de titular, datos aprobados, listas de lo que nunca se dice. |
| `brand/04-content-playbook.md` | Tipos de pieza, medidas, jerarquía y el ciclo semanal de contenido. |
| `tokens/tokens.css` | Variables CSS listas para usar. Toda pieza en código debe derivar de aquí. |
| `tokens/tokens.json` | Los mismos tokens en JSON, para herramientas que no leen CSS. |
| `examples/instagram-templates.html` | Cinco plantillas construidas con los tokens. Referencia de ejecución. |

## Reglas no negociables

1. Fondo negro. Nunca violeta, nunca gris claro, nunca blanco de fondo.
2. El violeta es acento: máximo un elemento por pieza, menos del 5% del área.
3. Geist nunca en bold. El peso visual ya está en la fuente.
4. Eyebrows y etiquetas siempre en IBM Plex Mono, mayúsculas.
5. Un dato concreto antes que un adjetivo. Si no hay dato, se reescribe el copy.
6. Fotografía real de equipo y eventos. Nada de stock corporativo.

## Qué NO hay aquí

- Logo en SVG/PNG y archivos de fuente. Se suben aparte en "Add fonts, logos and assets".
- Fotografía de banco. Las imágenes reales las provee el equipo (Daniele).
