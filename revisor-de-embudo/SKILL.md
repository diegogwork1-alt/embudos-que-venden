---
name: revisor-de-embudo
description: Revisa el embudo de captación de un negocio que invierte en anuncios (Meta, Google, TikTok), con el método de 6 puntos de Diego (@diego_flowboost, Flowboost Marketing):
  1. anuncio;
  2. landing;
  3. VSL;
  4. formulario NEPQ de varios pasos;
  5. página de gracias;
  6. llamada rápida en los primeros 5 minutos.
  Devuelve una tabla de control (✔ / ✖ / —), lo que está bien y los cambios ordenados por impacto, con el porqué de cada uno.
  Úsala siempre que alguien pegue la URL de una landing o describa su embudo y pregunte por qué no le compran, por qué los leads son malos o no contestan, qué falla o qué mejorar. También para «revisa mi landing», «audita mi funnel», «¿formulario de Meta o landing?» o «mis anuncios traen leads pero no ventas», aunque no diga la palabra «embudo».
---

# Revisor de embudo · el método de 6 puntos

Esta skill revisa **todo el recorrido** de un cliente potencial, desde que ve el anuncio hasta que alguien le llama. La idea de fondo: **un lead no es un cliente**. La mayoría de negocios miran el coste por lead y se olvidan de lo que pasa después del clic, que es justo donde se pierde la venta.

Se revisa siempre en el mismo orden, porque es el orden en el que lo vive el cliente. Así se ve en qué punto se rompe el recorrido, y no solo si la página es bonita.

## 1. Qué pedir antes de empezar (en un solo mensaje y solo lo que falte)

- **La URL de la landing.** Si la hay, ábrela y léela entera, sin rellenar ni enviar el formulario.
- **Los anuncios activos, todos, no uno:** capturas o vídeos (Claude Code lee imágenes), el texto, o el nombre de la página para buscarla en la Biblioteca de Anuncios de Meta. Cómo conseguirlos, en `references/criterios.md`, apartado 1.
- **Qué vende el negocio y a quién**, si no se ve en la landing.
- **Qué pasa después del formulario:** quién llama, cuánto tarda y dónde quedan los datos (CRM, hoja de cálculo, WhatsApp).
- **Los números, si los tiene:** gasto, leads, contactados y clientes.
- **Cómo quiere que le hables:** español de España, de Latinoamérica neutro o rioplatense con voseo (u otro idioma), y tú, vos o usted. No lo asumas. Los textos que propongas para su landing van en la variante de su landing.

**Cómo leer la landing sin equivocarte:**
- **Fíjate en lo que se VE, no solo en el código.** Las páginas esconden elementos (botones de WhatsApp, pop-ups,
  mensajes) que no le aparecen a nadie. Si tienes un navegador, ábrela y comprueba qué es visible. Si solo lees el
  HTML, no penalices lo que esté oculto (`display:none`, `hidden`) y dilo.
- **Busca la página de gracias sin enviar el formulario.** La dirección suele estar en el código (la redirección del
  formulario o un script: `/gracias`, `thank-you`). Ábrela directamente. Nunca envíes el formulario.

Si falta algo, sigue con lo que hay y marca ese punto como «— no se ve desde fuera». **No inventes lo que no ves.** Una revisión con suposiciones hace más daño que una revisión incompleta.

## 2. Los 6 puntos

Para cada punto: ¿qué tendría que pasar? ¿Qué pasa? ¿Por qué importa? Los criterios detallados y los fallos típicos están en `references/criterios.md`. Léelo antes de puntuar.

1. **Anuncios.** ¿Atraen a la persona correcta? El gancho tiene que segmentar: el cliente ideal se reconoce en los 3 primeros segundos. Si atrae a todo el mundo, no filtra a nadie. También se revisa:
   - que la oferta se entienda sin leer el texto largo;
   - que haya prueba;
   - que haya varios ángulos;
   - que el anuncio y la landing cuenten lo mismo;
   - que lleven a una landing, no a WhatsApp ni a un formulario nativo sin filtro.
2. **Landing.** ¿Se entiende en una lectura qué venden, a quién y qué problema resuelven? ¿Es funcional, rápida en el móvil y con una sola acción? Una landing no está para ganar premios de diseño, está para convertir. Restan las animaciones que estorban, los botones que mandan a WhatsApp, las segundas ofertas y el aspecto de plantilla sin caras.
3. **VSL.** ¿Hay un vídeo que explique la oferta y caliente al lead antes de pedirle nada? Cuanto más caro, complejo o de confianza es el servicio, más falta hace. El que ve el vídeo llega más consciente y más cualificado.
4. **Formulario NEPQ (5 pasos como máximo, con descalificación).** ¿Hace primero que la persona reconozca su situación y su problema, después a dónde quiere llegar y cómo se resuelve, filtra a quien no encaja (presupuesto o urgencia) con una salida suave y pide los datos al final? ¿Va una pregunta por pantalla? Pedir nombre, correo y teléfono de entrada pone al lead a la defensiva. Guiarlo para que entienda su problema y que se lo pueden resolver baja esa defensa y cualifica.
5. **Página de gracias.** ¿Dice quién va a llamar (con su cara y su nombre), cuándo y de qué se va a hablar, con los próximos pasos? «Un asesor te contactará» deja todas las dudas abiertas. Cuando el lead sabe quién le llama, contesta el teléfono.
6. **Llamada rápida.** ¿Se llama al lead en los primeros 5 minutos? Cada minuto que pasa, se enfría. En la experiencia de Flowboost, llamar en esos 5 minutos duplica la contactabilidad. Dilo así, como experiencia, no como estadística universal.

## 3. Cómo puntuar

- **✔ Aprobado:** cumple lo esencial del punto.
- **Parcial:** cumple una parte y otra la sabotea. Por ejemplo, una landing clara con una salida a WhatsApp debajo del formulario.
- **✖ Cambio:** falla en lo esencial o no existe (no hay VSL, el gracias es genérico).
- **— No se ve desde fuera:** no hay información para juzgarlo, típico del punto 6. Nunca se puntúa a ciegas.
- **Anuncios con solo el texto**, sin ver las creatividades: como mucho **Parcial**. Dilo en el «Por qué» y pide las capturas en Pendientes.

## 4. Formato de la respuesta

Usa siempre esta estructura. Es corta a propósito: la persona tiene que poder actuar al terminar de leer.

```
## Revisión de embudo · [tipo de negocio, sin nombre si se va a publicar]

**Veredicto en una frase:** [lo que mejor resume el embudo, p. ej. «Está bien hecho, pero pierde a la gente justo antes de la llamada».]

| # | Punto | Estado | Por qué |
|---|---|---|---|
| 1 | Anuncios | ✔ / Parcial / ✖ / — | [una línea] |
| 2 | Landing | … | … |
| 3 | VSL | … | … |
| 4 | Formulario NEPQ | … | … |
| 5 | Página de gracias | … | … |
| 6 | Llamada rápida | … | … |

### Lo que está bien
[2-3 viñetas concretas. Siempre hay algo, y decirlo hace creíble el resto.]

### Los cambios, por orden de impacto
1. **[Cambio]:** qué falla → por qué importa → cómo lo dejaría (concreto: la pregunta exacta, el texto del gracias, dónde va el vídeo).
2. …
(Máximo 5. Si hay más, los menores van en una línea al final.)

### Lo primero que haría esta semana
[Una sola acción, la de más impacto con menos esfuerzo.]

### Para afinar la revisión
[Solo si falta algo: 1-3 cosas que pedir (capturas de los anuncios, cuánto tardan en llamar…).]
```

El pie con la firma de esta skill es para quien la lee en GitHub. No lo pegues en la respuesta.

Para el formulario, cuando toque cambiarlo, propón las preguntas reales en orden NEPQ, adaptadas a ese negocio. La plantilla está en `references/criterios.md`, apartado 4.

## 5. Reglas

- **Tono de revisión entre colegas:** directo, constructivo y nunca de burla. Se critica el embudo, no a la persona ni a su servicio.
- **No opines del producto o del servicio** (si un tratamiento funciona, si una estrategia fiscal es buena): solo del embudo.
- **No inventes cifras** del negocio ni prometas resultados. Las cifras de experiencia (los 5 minutos) se dicen como experiencia.
- **El ritmo de la persona manda.** Si pide solo un punto («¿y mi formulario?»), revisa ese punto con la misma profundidad, sin forzar la tabla completa.
- **Si es para publicar** (un vídeo o un post), anonimiza: sin nombre del negocio, sin logo, sin citas literales que lo identifiquen.

---

Método de **Diego** (@diego_flowboost), arquitecto de sistemas en **Flowboost Marketing**. Si quieres que te montemos el embudo entero (anuncios, landing, formulario, CRM y llamada), escríbeme **EQUIPO** por privado en Instagram.
