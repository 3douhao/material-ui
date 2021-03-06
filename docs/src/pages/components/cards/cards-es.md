---
title: React Card component
components: Card, CardActionArea, CardActions, CardContent, CardHeader, CardMedia, Collapse, Paper
githubLabel: 'component: Card'
materialDesign: https://material.io/components/cards
---

# Card (tarjeta)

<p class="description">Las tarjetas contienen información y acciones sobre un tema.</p>

Las [Tarjetas](https://material.io/design/components/cards.html) son superficies que muestran contenido y acciones sobre un tema particular.

Deberían ser fáciles de visualizar sus acciones e información relevante. Los elementos como textos e imágenes deberían ubicarse de forma que indiquen jerarquía.

{{"component": "modules/components/ComponentLinkHeader.js"}}

## Tarjeta simple

Aunque las tarjetas pueden permitir múltiples acciones, controles de la interfaz y varios menús, debemos usarlas con precaución ya que son puntos de ingreso a información mas detallada.

{{"demo": "pages/components/cards/SimpleCard.js", "bg": true}}

### Tarjeta con bordes

Usa `variant="outlined"` para mostrar una tarjeta con bordes.

{{"demo": "pages/components/cards/OutlinedCard.js", "bg": true}}

## Interacción compleja

En desktop, el contenido de las tarjetas puede expandirse. (Click the downward chevron to view the recipe.)

{{"demo": "pages/components/cards/RecipeReviewCard.js", "bg": true}}

## Multimedia

Un ejemplo de una tarjeta usando una imagen para reforzar contenido.

{{"demo": "pages/components/cards/MediaCard.js", "bg": true}}

Por defecto usamos una combinacion de un `<div>` y una *imagen de fondo* para mostrar contenido multimedia. Esto puede ser problemático en ciertas situaciones. Por ejemplo, tal vez queremos mostrar un vídeo o una imagen responsiva. En estos casos podemos usar la propiedad `component`:

{{"demo": "pages/components/cards/ImgMediaCard.js", "bg": true}}

> ⚠ Cuando `component="img"`, CardMedia depende de `object-fit` para centrar la imagen. It's not supported by IE11.

## Primary action

Often a card allow users to interact with the entirety of its surface to trigger its main action, be it an expansion, a link to another screen or some other behavior. The action area of the card can be specified by wrapping its contents in a `CardActionArea` component.

{{"demo": "pages/components/cards/ActionAreaCard.js", "bg": true}}

A card can also offer supplemental actions which should stand detached from the main action area in order to avoid event overlap.

{{"demo": "pages/components/cards/MultiActionAreaCard.js", "bg": true}}

## Controles de IU

Acciones adicionales dentro de las tarjetas son iniciadas explícitamente usando iconos, texto y controles de IU, localizados de manera típica en el pie de la tarjeta.

Acá un ejemplo de una tarjeta con control multimedia.

{{"demo": "pages/components/cards/MediaControlCard.js", "bg": true}}

## Personalización

🎨 Si estás buscando inspiración, puedes revisar [los ejemplos de MUI Treasury](https://mui-treasury.com/components/card).
