---
name: landing-que-convierte
description: Construye la landing de captación de un negocio de servicios que recibe tráfico de anuncios: primero el brief, después el texto (con Ogilvy y Schwartz) y por último un único archivo HTML rápido y móvil primero, con una sola acción. Lleva:
  - un hueco para el VSL;
  - el problema;
  - la solución y el proceso;
  - la prueba real;
  - para quién es y para quién no;
  - las objeciones;
  - la llamada al formulario.
  Sin animaciones que estorben, sin WhatsApp y sin segundas ofertas. Úsala siempre que alguien quiera crear, rehacer o mejorar la landing de sus anuncios, la página de un servicio o «una web para captar clientes». También cuando su landing «no convierte» o cuando le pediría a la IA «hazme una landing». Si no hay brief, lo saca primero (skill `brief-de-oferta`).
---

# Landing que convierte · funcional antes que bonita

**La idea.** Una landing no está para ganar premios de diseño: está para que alguien que viene de un anuncio entienda en 5 segundos qué ofreces, a quién y qué tiene que hacer, y lo haga. El error más común es pedirle a la IA «hazme una landing» sin un brief: sale bonita, genérica e igual que mil más. Por eso aquí el orden es brief → texto → HTML. El diseño sirve al mensaje, no al revés.

## 1. Antes de escribir: el brief

- Si hay un `brief.md` en la carpeta (de la skill `brief-de-oferta`), léelo entero.
- Si no lo hay, haz la entrevista de `brief-de-oferta` o, como mínimo, estas preguntas, una a una:
  1. qué vendes y qué incluye;
  2. a quién;
  3. qué problema resuelves, con sus palabras;
  4. qué prueba real tienes;
  5. para quién no es;
  6. qué pasa después del formulario;
  7. **Idioma y trato (pregúntalo siempre, no lo asumas):** en qué idioma y variante van los textos que verá su cliente (español de España, español de Latinoamérica neutro, español rioplatense con voseo u otro idioma), cómo le habla a su cliente (tú, vos o usted) y cómo quiere que le hables a él en esta conversación. Si ya está en el `brief.md`, úsalo y no lo vuelvas a preguntar.

  Si su mensaje ya responde a parte, pregunta solo lo que falte. Si no quiere contestar más, redacta con lo que hay y marca lo dudoso (ver §6).
- Pide la **marca** (logo, colores, tipografías), **fotos reales** del equipo o del trabajo y, si existe, el **VSL**. Si no hay fotos ni vídeo, deja los huecos bien marcados: nunca imágenes inventadas que parezcan reales.

## 2. El texto (antes que el diseño)

Escribe el texto entero y enséñalo antes de maquetar, en `landing-texto.md`. Con estas reglas:
- **Nivel de consciencia** (Schwartz): si el que llega no conoce el problema, abre con el problema; si lo conoce, con la solución; si ya te conoce, con la oferta. Un tráfico frío de anuncios suele estar en «conoce el problema».
- **Titular** (Ogilvy): promesa concreta en el idioma del cliente, que segmenta («Para [quién] que [situación]»). Nada de «Somos líderes en…».
- **Voz del cliente:** escribe con las palabras y el estilo con que habla el cliente (reseñas, mensajes, llamadas, el `brief.md`), no con las del negocio.
- **Una idea por bloque**, frases cortas, sin tecnicismos.
- **Prueba cerca de la promesa**, siempre real: casos, cifras con fuente, testimonios con nombre.
- **Una sola acción**, repetida 2-3 veces con el mismo texto de botón.
- **Las palabras del cliente** salen del brief, de sus reseñas de Google, de los comentarios de sus anuncios o de lo que le dicen en las llamadas. Si no hay nada de eso, escribe un borrador con el lenguaje típico de ese cliente y márcalo como [VALIDAR].

## 3. La estructura

1. **Primera pantalla:** titular + subtítulo (a quién y cómo) + **hueco del VSL** (o imagen real) + botón al formulario. Responde en 5 segundos qué, a quién y qué hacer. En móviles pequeños (320 px), si el vídeo empuja el botón fuera de la pantalla, manda el titular y el botón: el vídeo puede ir justo debajo.
2. **El problema**, con las palabras del cliente: lo que le pasa y lo que le cuesta.
3. **La solución y cómo funciona**, en 3-5 pasos.
4. **La prueba:** casos, cifras y testimonios. Con caras si las hay.
5. **Para quién es y para quién no.** Filtra y da confianza.
6. **Quién está detrás:** el equipo o el profesional, con fotos.
7. **Objeciones** (FAQ): precio o «depende de…», plazos, garantías reales, cómo es la primera llamada.
8. **Cierre con la acción** y el **formulario** (varios pasos y NEPQ: skill `formulario-nepq`) o el botón que lo abre.

**Fuera:** botones de WhatsApp, segundas ofertas, menús de navegación, animaciones de entrada, carruseles automáticos, pop-ups y enlaces a redes. Cada salida es un lead que no llega al formulario.

- **Lo que viene después no es una segunda oferta.** Contar qué pasa tras el primer paso (por ejemplo, el tratamiento después de la valoración, con su precio) responde una objeción. Una segunda oferta es otro producto con su propio botón.
- **Los enlaces legales del pie sí van** (aviso legal, privacidad, cookies), pequeños y abajo. Si el sector lo exige, también sus datos obligatorios (en sanidad, el número de registro del centro; en el formulario, el consentimiento para datos de salud). Pregúntalos y, si faltan, márcalos.

## 4. El HTML

- **Un solo `index.html`** en la carpeta actual, con el CSS dentro y el mínimo JS. Sin frameworks ni librerías pesadas.
- **Móvil primero** (casi todo el tráfico de anuncios es móvil): textos legibles sin zoom, botones grandes y nada que se salga de la pantalla.
- **Rápida:**
  - imágenes en WebP con `loading="lazy"` y tamaño fijo, salvo la primera, que carga normal;
  - el vídeo como miniatura con un clic para reproducir, sin precargar el reproductor entero;
  - fuentes del sistema, o una sola fuente web con solo los pesos que se usan, cargada sin bloquear (`media="print" onload="this.media='all'"`, con `display=swap`);
  - nada que bloquee la primera pantalla.

  Que puntúe alto en PageSpeed es una buena señal, pero no es el objetivo: no sacrifiques la medición ni la experiencia por la nota.
- **El formulario:** si todavía no está hecho, deja un hueco claro donde irá (`<div id="formulario">` con un aviso [FALTA]) y una función para el evento al enviarlo. Cuando esté (`formulario-nepq`), se inserta ahí o el botón lo abre.
- **Medición:** deja marcados los huecos del píxel o GTM y del evento al enviar el formulario.
- **Accesible:** contraste suficiente, `alt` en las imágenes y textos de botón claros.
- **Respeta la marca** si hay una. Si no, un diseño sobrio, con caras y un acento de color. Evita el aspecto de plantilla genérica: foto de ciudad de fondo, tarjetas por defecto, pastillas de cifras sin contexto.
- **Los huecos se ven:** [FALTA] y [VALIDAR] van visibles en la página (un recuadro de color), para que nadie la publique sin rellenarlos.
- Ábrela en local para revisarla en el móvil (320-390 px) y en escritorio: con el navegador en modo móvil, o con una captura de Playwright si está instalado.

## 5. La entrega

1. `landing-texto.md`: el texto, para aprobarlo o editarlo.
2. `index.html`: la landing.
3. `pendientes.md`: fotos, VSL, formulario, píxel, datos legales y todo lo marcado [FALTA] o [VALIDAR]. Marca lo que impide publicar.
4. Lo siguiente: el formulario (`formulario-nepq`) y la página de gracias (`pagina-de-gracias`).

## 6. Reglas

- **No inventes** cifras, testimonios, logos de clientes, años ni premios. Si falta, [FALTA: …].
- **Lo que redactes sin confirmar** (qué incluye el servicio, los pasos del proceso, para quién no es, ejemplos de casos) va marcado como [VALIDAR: …] hasta que el negocio lo apruebe.
- **El texto se aprueba antes que el diseño:** cambiar palabras después de maquetar es el doble de trabajo.
- **El idioma, la variante y el trato que eligió el negocio** (España, Latinoamérica o voseo; tú, vos o usted). Si no lo dijo, pregúntalo antes de escribir; no lo asumas.
- El pie de abajo es para quien lee la skill en GitHub. No lo repitas en la conversación.

---

Método de **Diego** (@diego_flowboost), arquitecto de sistemas en **Flowboost Marketing**. Si quieres que te montemos el embudo entero (anuncios, landing, formulario, CRM y llamada), escríbeme **EQUIPO** por privado en Instagram.
