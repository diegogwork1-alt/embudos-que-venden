---
name: brief-de-oferta
description: Entrevista al dueño de un negocio, pregunta por pregunta, para sacar el brief de su oferta antes de construir la landing, el formulario o la página de gracias, o antes de escribir anuncios o el guion de un VSL. Claude hace las preguntas una a una, repregunta cuando la respuesta es vaga, guarda un borrador después de cada bloque y al final deja `brief.md` en la carpeta actual. El brief cubre qué vende, a quién, qué problema resuelve, por qué duele, qué prueba tiene, qué lo diferencia, el proceso del cliente, qué no se puede decir y el antes y el después. Es la base de las skills `landing-que-convierte`, `formulario-nepq` y `pagina-de-gracias`. Úsala cuando alguien diga «quiero hacer una landing / anuncios / un VSL», «ayúdame con mi oferta», «no sé cómo explicar lo que vendo» o «hazme el brief», o antes de escribir cualquier texto de venta si no hay brief.
---

# Brief de oferta · la entrevista antes de construir nada

**La idea.** Casi todo el mundo abre la IA y pide «hazme una landing para mi negocio». La IA rellena lo que no sabe con frases genéricas y sale una página que podría ser de cualquiera. Antes de construir hay que entender qué vendes, a quién, qué problema resuelves y por qué te deberían creer. Esta skill saca eso con una entrevista. La persona habla de su negocio y Claude hace el trabajo de ordenarlo.

## 1. Antes de la primera pregunta

- **Si ya existe `brief.md` en la carpeta**, léelo. Si está «en curso», resume en dos líneas lo que hay y sigue desde la siguiente pregunta sin respuesta. Si está completo, pregunta si quiere actualizarlo.
- **Aprovecha lo que ya ha contado.** Si en su primer mensaje dijo qué vende o a quién, no se lo vuelvas a preguntar: confírmalo («Me dices que es una academia de inglés online para profesionales, ¿correcto?») y pasa a lo que falta.
- **El idioma y el trato, en el mensaje de apertura y siempre preguntados, nunca deducidos** (quien escribe no tiene por qué hablar como su cliente):
  1. en qué idioma y variante van a estar los textos que lea su cliente: español de España, español de Latinoamérica neutro, español rioplatense con voseo u otro idioma;
  2. cómo le habla a su cliente: tú, vos o usted;
  3. cómo quiere que le hables a él durante la entrevista.

  Entrevista como pidió y escribe el brief en la variante de sus textos.
- **Mensaje de apertura, corto:**
  - las tres preguntas del idioma y el trato, para contestar ya;
  - son 22 preguntas, unos 30-40 minutos escribiendo;
  - se guarda un borrador al terminar cada bloque, así que puede parar cuando quiera y seguir otro día;
  - si va a hacer también el formulario y la página de gracias, hay 5 preguntas más al final (bloque G), para no tener que repetirlas luego. Pregúntale si las incluyes y numera con el total real desde el principio («Pregunta 4 de 27»).

## 2. Cómo se hace la entrevista

- **Una pregunta cada vez**, numerada, y espera la respuesta. Juntas, abruman y salen respuestas cortas. Si una pregunta tiene una segunda parte que es solo un dato (un sí o no, un nombre), puede ir en el mismo mensaje.
- **Explica en una línea por qué preguntas** cuando no sea obvio: «Te lo pregunto porque esto es lo que va en el titular».
- **Repregunta una vez si la respuesta es vaga.** «Damos un servicio de calidad» no sirve: «¿Qué haces que otro no haga? Dame un ejemplo de un cliente concreto». Si tras la repregunta sigue vaga, apúntala tal cual, añádela a Pendientes como «concretar» y sigue: dos repreguntas seguidas suenan a examen.
- **Pide ejemplos y palabras literales de sus clientes** (reseñas, mensajes, lo que le dicen en las llamadas). Son el mejor material para los anuncios. Si solo lo recuerda a medias, apúntalo como paráfrasis, sin comillas y con «(de memoria)», para que nadie lo use luego como cita real.
- **No inventes respuestas.** Puedes orientar (dónde mirar a su competencia: la Biblioteca de Anuncios de Meta o buscar su servicio en Google), pero no des nombres ni datos por él. Si no lo sabe, va a [PENDIENTE] y se sigue.
- **Si clasifica algo de forma rara**, respétalo y pregúntalo una vez («Vaughan, ¿lo ves como competencia directa o como otra cosa?»). No le corrijas.
- **Deja saltar o volver atrás:** «Saltamos esta y la vemos al final».
- **Guarda el borrador al terminar cada bloque** (y si dice «paro aquí»): escribe `brief.md` con lo que haya, `Estado: en curso · última pregunta: N`. Dilo en media línea: «Guardado, seguimos con la prueba».

## 3. Las preguntas

**Bloque A · La oferta**
1. ¿Cómo se llama tu negocio y qué vendes, en una frase, como se lo dirías a un amigo?
2. ¿Qué problema resuelve?
3. ¿A quién se lo resuelves? Cuéntame su situación, no solo su edad: qué tiene y qué le falta.
4. ¿Qué incluye exactamente lo que vendes? Qué recibe el cliente, en qué formato y durante cuánto tiempo.

**Bloque B · El dolor y el deseo**
5. ¿Qué le cuesta HOY a tu cliente seguir con ese problema? En dinero, tiempo o tranquilidad.
6. Si el problema estuviera resuelto, ¿cómo sería su día a día?
7. ¿Qué te dicen tus clientes cuando te contactan por primera vez? Las palabras exactas, si las recuerdas.
8. ¿Qué les frena para contratarte? ¿Qué objeciones oyes más?

**Bloque C · La prueba**
9. ¿Cómo demuestras que puedes resolverlo? Casos, cifras, años, clientes, reseñas, certificados, prensa. Solo lo real, y dime dónde se puede ver (Google, tu web, un contrato…).
10. ¿Tienes un cliente concreto con un antes y un después que puedas contar? Si es que sí: ¿tienes su permiso para usar su nombre (o su cara) en público?
11. ¿Cómo nació tu negocio y por qué?

**Bloque D · El mercado**
12. ¿Quién es tu competencia más directa?
13. ¿Qué hace tu cliente en lugar de contratarte? Hacerlo él, no hacer nada, una app, otra solución… y qué ha probado ya.
14. ¿Qué haces tú que ellos no hacen?
15. Tu marca en tres palabras que sí, y tres que nunca querrías que dijeran de ella.

**Bloque E · El proceso**
16. Paso a paso, como para un niño: ¿qué hace el cliente desde que te conoce hasta que consigue el resultado?
17. Cuando ya quiere comprar, ¿qué tiene que hacer (llamada, visita, presupuesto…) y quién le atiende?
18. ¿Precio o rango? ¿Se puede poner en la página o mejor «depende de…»?
19. ¿Para quién NO es tu servicio? ¿A quién no quieres atender?
20. ¿Hay cosas que no puedes decir o prometer, por ley o por tu sector? (salud, finanzas, legal, resultados garantizados…)

**Bloque F · El cierre**
21. Si tu cliente no hace nada, ¿adónde le lleva eso dentro de un año? (La 5 es lo que le cuesta hoy; esta, hacia dónde va.)
22. Con lo que me has contado, propón tú el antes y el después en una frase cada uno, y pregunta: «¿Lo cambiarías?».

**Bloque G · Para el formulario y la página de gracias** (si lo ha pedido)
23. A quien no encaja (poco presupuesto, otra zona, solo mirando), ¿qué le puedes ofrecer en vez de una llamada? Un contenido, una guía, otro servicio o «vuelve cuando…».
24. ¿Quién hace la llamada? Nombre, cargo y una foto.
25. ¿Desde qué número o prefijo llamáis?
26. ¿Cuánto tardáis en llamar a un lead nuevo, y en qué días y horas llamáis? Lo que pasa de verdad, no lo ideal.
27. ¿De qué va esa llamada, cuánto dura, qué sale de ella y qué conviene que el cliente tenga a mano?

## 4. La entrega

Al terminar, escribe `brief.md` en la carpeta actual (sustituye el borrador):

```
# Brief · [Negocio]
Fecha: [hoy] · Estado: [completo / con pendientes]
Idioma de los textos: [España / Latinoamérica neutro / rioplatense con voseo / otro] · Trato con sus clientes: [tú / vos / usted] · Cómo hablarle al dueño: [lo que pidió]

## En una frase
[Qué vende, a quién y el resultado, en una línea.]

## 1. La oferta            (1-4)
## 2. El dolor y el deseo   (5-8)
## 3. La prueba            (9-11)
## 4. El mercado           (12-15)
## 5. El proceso           (16-20)
## 6. El cierre            (21-22)
## 7. Formulario y llamada (23-27, si se hizo)
## Pendientes
- [lo que quedó en PENDIENTE o «concretar», para completarlo]
```

**Cómo se escribe cada sección:** en viñetas cortas, en primera persona del dueño («Ayudo a…»), con sus palabras y ordenado. Las marcas van al final de la viñeta, entre corchetes. Por ejemplo:

```
## 3. La prueba
- He dado clase a más de 340 alumnos desde 2019. [lo dice el dueño · comprobar antes de publicar]
- 4,8 en Google con 96 reseñas. [comprobable: ficha de Google]
- Raquel, jefa de proyecto: «Llevaba dos años sin abrir la boca en los weekly con Alemania». [permiso para nombrarla: sí]
- Muchos me dicen que se bloquean cuando les preguntan algo en inglés. (de memoria)
- Los alumnos suelen notar el cambio hacia el segundo mes. [Inferencia]
```

- Puedes redactar mejor, pero **sin añadir hechos que no dijo**. Lo que deduzcas, márcalo como [Inferencia].
- Cada prueba lleva de dónde sale: **[comprobable: …]** si se puede ver en algún sitio, o **[lo dice el dueño · comprobar antes de publicar]** si solo lo afirma él.

**Al final, en la conversación**, una línea con qué se puede hacer ahora con el brief:
- la landing (`landing-que-convierte`);
- el formulario (`formulario-nepq`);
- la página de gracias (`pagina-de-gracias`).

Para los anuncios y el guion del VSL, el brief es el material de partida: los bloques B y C dan los ganchos y la prueba.

## 5. Reglas

- **Nunca inventes** cifras, testimonios, casos, precios ni nombres. Lo que no esté, va a Pendientes.
- **Sus palabras valen más que las tuyas:** guarda las frases literales del cliente y del dueño.
- **El idioma y la variante del negocio** (España o Latinoamérica, tú o usted), en la entrevista y en el brief.
- El pie de abajo es para quien lee la skill en GitHub. No lo repitas en la conversación.

---

Método de **Diego** (@diego_flowboost), arquitecto de sistemas en **Flowboost Marketing**. Si quieres que te montemos el embudo entero, escríbeme **EQUIPO** por privado en Instagram.
