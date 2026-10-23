---
name: copy-mining
description: Hace un copy mining de las reseñas de un negocio. La persona pega sus reseñas (Google, Trustpilot, Amazon, mensajes de clientes, transcripciones de llamadas…) o las de su competencia, y Claude saca las palabras exactas con las que sus clientes describen por qué compraron, qué temían antes y qué les encantó después, para escribir anuncios, landings y guiones con ellas. Entrega:
  - el corpus limpio, cuántas reseñas hay y qué limitaciones tiene;
  - motivaciones, valores y ansiedades con su recuento;
  - los patrones de lenguaje con citas literales y las frases con más potencial;
  - la matriz voz del cliente, los territorios publicitarios, la big idea y 50 líneas de anuncio;
  - un informe en un solo HTML, imprimible a PDF, y el mismo contenido en .md.
  Si no tiene las reseñas a mano, le explica cómo conseguirlas. Úsala cuando alguien pegue reseñas o comentarios de clientes, cuando pida «copy mining», «review mining», «voz del cliente» o «voice of customer», cuando no sepa qué poner en sus anuncios, o cuando quiera escribir con las palabras de sus clientes en vez de con las suyas.
---

# Copy mining · tus anuncios con las palabras de tus clientes

**La idea.** Cuando un negocio escribe sus anuncios, escribe lo que cree que vende: «atención personalizada», «profesionales con experiencia», «calidad». Lo mismo que pone su competencia. Sus clientes, en cambio, ya escribieron el anuncio que funciona: está en sus reseñas, con sus palabras, sus miedos y lo que les sorprendió. El copy mining es leer esas reseñas con método y sacar de ellas el material de los anuncios.

**Para qué sirve.** Para dejar de adivinar qué poner en un anuncio. El que lo lee se reconoce porque lo escribió alguien como él. Un ejemplo real: en las reseñas de Vibrana, una agencia de viajes en grupo, dos clientes escribieron «Después de estar algo escarmentada con los viajes en grupo…» y «Nunca imaginé que haría un viaje en grupo». De ahí salió su big idea: **«El viaje en grupo para personas que no quieren hacer un viaje en grupo»**. Ningún equipo de marketing la habría escrito desde una mesa.

**No hacen falta cientos de reseñas.** Home Server, una empresa de cuidado de personas mayores, tenía 225 reseñas (134 con texto): sus clientes escribían «en pocos días tenía una cuidadora» o «facilitar los trámites», y en las críticas aparecía el miedo por la seguridad y el trato de su familiar. Vibrana tenía solo 15 (12 con texto), y con eso ya salieron los miedos, los ángulos y la big idea. Con unas 15 reseñas ya entiendes qué quiere tu cliente, qué teme y qué valora.

**El método.** Es el sistema de Kris Sugatan, tal como lo explican en Ad World Prime: las reseñas son el único estudio de mercado que hacen para producir anuncios. Cada reseña se lee con tres preguntas:
1. **¿Por qué compró?** Lo que le hizo decidirse.
2. **¿Qué temía antes?** El miedo o la duda que tenía antes de comprar o de recibir el servicio.
3. **¿Qué le encantó después?** Lo que destaca una vez vivido.

Con eso se sacan las motivaciones, los valores y las ansiedades, se cuentan, se ordenan, y de ahí salen los mensajes: hasta 50 líneas de anuncio.

## 1. Qué preguntar antes (en un solo mensaje, solo lo que falte)

Si hay un `brief.md` en la carpeta (de la skill `brief-de-oferta`), léelo primero y pregunta solo lo que falte.

1. **Qué vende el negocio y a quién**, en una frase, y el nombre de la marca (para las líneas de anuncio).
2. **De quién son las reseñas:** del propio negocio, de su competencia o de las dos cosas. Si hay de varias fuentes, de dónde sale cada bloque.
3. **Las reseñas.** Si no las tiene a mano, explícale cómo conseguirlas con la sección 2.
4. **Para qué las quiere usar primero:** anuncios de Meta, la landing, guiones de vídeo, el formulario… Cambia qué líneas van primero, no el análisis.
5. **Idioma y trato (pregúntalo siempre, no lo asumas):** en qué idioma y variante van las líneas de anuncio (español de España, español de Latinoamérica neutro, español rioplatense con voseo u otro idioma), cómo le habla a su cliente (tú, vos o usted) y cómo quiere que le hables a él en esta conversación. Si ya está en el `brief.md`, úsalo y no lo vuelvas a preguntar. Las citas de los clientes van siempre tal cual, en su idioma original.

## 2. Cómo conseguir las reseñas

Si la persona ya las pegó o te pasó un archivo, salta al paso 3. Si no, explícale estas opciones, de la más fácil a la más trabajosa:

1. **Google Maps, la opción fácil.** La extensión de Chrome [Maps Reviews Exporter: Reviews to CSV & JSON](https://chromewebstore.google.com/detail/maps-reviews-exporter-rev/diboglcabfkcinmhjnmlmeplilighncl). Según su ficha, exporta las reseñas de cualquier sitio de Google Maps con la puntuación, la fecha, el texto, el autor, la respuesta del dueño, las fotos y los «me gusta».
   - Pasos: instalarla en Chrome, abrir la ficha del negocio en Google Maps, exportar y pegar el CSV en la conversación o arrastrar el archivo a Claude Code.
   - La versión gratis exporta hasta 50 reseñas por vez, en CSV. Para más reseñas o para JSON tiene una versión de pago (así lo dice su ficha en octubre de 2026; puede cambiar). Comprueba cuántas filas trae el archivo frente al total de la ficha: si faltan muchas, vuelve a exportar o completa a mano.
   - La skill acepta CSV y JSON, y se queda solo con el texto, la puntuación y la fecha. El nombre del autor no se usa.
2. **Copiar y pegar a mano**, para pocas reseñas. Ojo: las que están cortadas con «Más» hay que abrirlas antes de copiar, porque si no quedan incompletas y los recuentos salen por debajo. Pasó en el informe de Vibrana: 8 de sus 12 reseñas con texto estaban cortadas.
3. **Otras fuentes del propio negocio:**
   - Trustpilot, Amazon, Doctoralia, TripAdvisor u otra plataforma de su sector (muchas dejan exportar o copiar);
   - mensajes de WhatsApp o correos de clientes contentos, con su permiso;
   - transcripciones de llamadas de venta;
   - comentarios en redes;
   - respuestas abiertas de encuestas.
4. **La competencia y el mercado.** Las reseñas de sus competidores en Google Maps (con la misma extensión), Reddit y foros del sector. Sirven sobre todo para las ansiedades: lo que se le critica a la competencia es lo que tu cliente teme. Se analizan aparte y se marca de dónde sale cada cita.
5. **¿Puede sacarlas la skill sola?** De Google Maps, no: la página carga dinámica y automatizarla va contra sus condiciones, así que no lo intentes ni lo prometas. Si Claude Code tiene acceso a la web, puede leer una página pública que se abra sin iniciar sesión (por ejemplo, el perfil de una empresa en Trustpilot). Si no se puede, pide el archivo o el texto.

## 3. Limpiar el corpus y contar

Antes de analizar nada:

- **Quita el ruido de la interfaz:** «Me gusta», «Compartir», «Más», «Nueva», «Local Guide», número de reseñas del autor, fotos, fechas sueltas y cualquier texto que no haya escrito el cliente. Las respuestas del dueño no cuentan como voz del cliente.
- **Quita duplicados** y separa las reseñas sin texto (solo estrellas).
- **Anonimiza:** cada reseña pasa a ser R1, R2, R3… (o C1, C2… si son de la competencia). El nombre de quien la escribió no se usa en ningún sitio.
- **Marca las cortadas** («…», «Más») como truncadas.
- **Cuenta y dilo:** reseñas detectadas, con texto, sin texto, truncadas, palabras aproximadas, idioma, reparto de estrellas y rango de fechas si lo hay.
- **Di las limitaciones.** Si hay truncadas, los recuentos son mínimos, no frecuencias definitivas. Si casi todas son de 5 estrellas, las ansiedades serán sobre todo latentes (ver el paso 5).
- **Pocas reseñas no es un problema: sigue.** Con unas 15 reseñas con texto ya se ven los miedos, lo que valoran y los ángulos (el informe de Vibrana salió de 12 con texto). Con menos también se hace: avisa de que los recuentos son orientativos y propón sumar otras fuentes (mensajes de clientes, transcripciones de llamadas, las reseñas de la competencia). No desanimes a nadie por tener pocas.

## 4. Las tres preguntas, reseña por reseña

Para cada reseña con texto, anota en una tabla interna:

| ID | ¿Por qué compró? | ¿Qué temía antes? | ¿Qué le encantó después? |
|---|---|---|---|
| R3 | «prometía una experiencia diferente» | «algo escarmentada con los viajes en grupo» | «vivir una Indonesia como…» (truncada) |

- Cada celda es una **cita literal** de la reseña. Si la reseña no lo dice, la celda queda en «no lo dice». No la rellenes con lo que «se entiende».
- Esta tabla es la base de todo lo demás. Va en el informe, en el apartado de las tres preguntas.

## 5. El análisis

Todo lo que sale de aquí tiene dos capas, y en el informe se distinguen a la vista:
- **Lo que dicen los clientes:** citas literales con su ID (R3, R7) y recuentos.
- **La lectura:** lo que interpretas tú. Va marcado como «Interpretación» y nunca se presenta como algo que dijo un cliente.

Por orden:

1. **Motivaciones, valores y ansiedades, con su recuento.** Agrupa en categorías cortas (5-10 por bloque). La unidad es **el número de reseñas con evidencia** del concepto, no las veces que aparece una palabra. Una reseña puede contar en varias categorías. Cada categoría lleva al menos una cita y los IDs donde aparece.
   *Para qué sirve:* las motivaciones dan el gancho y la promesa del anuncio; los valores, lo que el anuncio tiene que demostrar; las ansiedades, las objeciones.
2. **Ansiedades explícitas y latentes.** Las explícitas las dice el cliente («escarmentada con los viajes en grupo»). Las latentes se deducen de lo que el cliente remarca: si cinco personas destacan la organización, el miedo de fondo es la improvisación. Las latentes van marcadas como interpretación.
   *Para qué sirve:* son las objeciones que el anuncio y la landing contestan antes de que el cliente las pregunte. Si el anuncio no las toca, las piensa igual y no compra.
3. **Patrones de lenguaje.** Tabla: patrón · cuántas reseñas · citas literales · fuerza para el copy (de 1 a 5 estrellas, y en una línea por qué).
   *Para qué sirve:* dice qué temas repetir en toda la comunicación, porque son los que más clientes mencionan.
4. **Frases con más potencial.** Entre 10 y 20 expresiones **copiadas tal cual del corpus**, con lo que comunican (diferenciación, objeción, transformación, confianza…). Si una frase no está escrita así en ninguna reseña, no va en esta lista.
   *Para qué sirve:* es el texto de tus anuncios y de tu landing, con las palabras de tus clientes. En Home Server: «en pocos días tenía una cuidadora», «facilitar los trámites».
5. **Estructuras narrativas que se repiten:** «Pensaba X → descubrí Y», «No es X → es Y», «Característica → consecuencia emocional»… Cada una con su ejemplo literal.
   *Para qué sirve:* son estructuras de anuncio que tus clientes ya usan al contar su experiencia: el «Pensaba X → hasta que…» sirve de guion de vídeo; el «No es X → es Y», de titular.
6. **Matriz voz del cliente.** Territorio (organización, cuidado, confianza, precio, resultado…) · palabras y expresiones detectadas.
   *Para qué sirve:* es el vocabulario de cada tema. Cuando escribas sobre organización, precio o trato, usa sus palabras y no las tuyas.
7. **El hallazgo: insight central y transformación.** Qué resuelve la ansiedad más fuerte, dicho como lo dicen los clientes, y la transformación: antes (cita) → lo que lo cambia (el mecanismo) → después (cita). Suele tener la forma «No es X → es Y» o «No solo X → también Y». En Vibrana, el miedo era «escarmentada con los viajes en grupo» y lo que lo resolvía, en 6 reseñas, era «no es un viaje en grupo al uso». En Home Server: no solo encontrar cuidadora, también quitarse trámites y dudas. Es interpretación apoyada en citas. Si se puede, resúmelo en una ecuación de valor (en Vibrana: organización → tranquilidad → libertad para vivir el viaje).
   *Para qué sirve:* es la diferencia que el anuncio tiene que contar. Sin hallazgo, el anuncio dice lo mismo que la competencia.
8. **Territorios publicitarios.** De 3 a 5, ordenados por potencial. Cada uno nace de una cita y dice en una línea por qué tiene fuerza.
   *Para qué sirve:* cada territorio es una línea de anuncios para probar por separado.
9. **Big idea.** Una frase que une la ansiedad más fuerte, lo que diferencia al negocio y la prueba de los clientes. Dila con lo que la sostiene.
   *Para qué sirve:* es el ángulo de toda la campaña. Los anuncios, la landing y el vídeo la cuentan de formas distintas.
10. **50 líneas de anuncio.** Agrupadas por territorio, en el idioma y el trato elegidos. Pueden reescribir el lenguaje del cliente, pero:
    - no prometen nada que ningún cliente haya dicho;
    - no meten cifras, plazos ni garantías que no estén en el corpus o en el brief;
    - si una línea lleva una frase entre comillas, la frase es literal del corpus.

    Si es para Meta, marca las 5 que probarías primero y por qué.
   *Para qué sirve:* son ganchos y titulares para probar en los anuncios.

Si las reseñas son de la competencia, el análisis es el mismo, pero las líneas de anuncio son para el negocio de la persona. Nunca nombran a la competencia ni usan sus reseñas como si fueran propias.

## 6. La entrega

Dos archivos en la carpeta actual, con el mismo contenido:

- **`copy-mining-[marca].html`**: el informe, en un solo archivo, sin dependencias, que se imprime a PDF desde el navegador (A4 apaisado). Parte de `assets/plantilla.html`: ya trae los estilos, la estructura y las barras de los gráficos. Pon cada sección en una página nueva cuando no quepa.
- **`copy-mining-[marca].md`**: lo mismo en texto, para copiar líneas a otros documentos o pasárselo a otra herramienta.

La estructura del informe (cada sección empieza con una línea «Para qué sirve», la misma del paso 5, para que quien lo lea sepa qué hacer con ella):

1. **Portada:** marca, cifras del corpus (reseñas, con texto, valoración, palabras), big idea y promesa que emerge.
2. **Diagnóstico del corpus:** cómo se limpió, las cifras, las señales que aparecen y las **limitaciones**.
3. **Las tres preguntas:** la tabla del paso 4.
4. **Resumen:** motivaciones, valores y ansiedades en tres columnas, con su recuento, y una línea de lectura.
5. **Patrones de lenguaje** y el patrón narrativo de más valor.
6. **Frases con más potencial** y estructuras narrativas.
7. **Matriz voz del cliente** e insight central.
8. **Motivaciones, valores y ansiedades en detalle**, con las citas.
9. **Las ansiedades:** explícitas, latentes y la transformación antes → mecanismo → después.
10. **Gráficos:** una barra por categoría, de motivaciones, valores y ansiedades, con su número.
11. **Territorios publicitarios y big idea.**
12. **Las 50 líneas de anuncio.**
13. **Apéndice:** el corpus usado, anonimizado (ID, texto visible, estado: completa o truncada).

En la conversación, resume en pocas líneas: cuántas reseñas, las limitaciones, la big idea, los 3 territorios más fuertes y las 5 líneas que probarías primero. Y dile dónde están los dos archivos.

## 7. Cómo usarlo después

- **Anuncios:** las líneas de anuncio son ganchos y titulares. Las ansiedades son las objeciones que el anuncio tiene que contestar.
- **Landing:** la big idea va en el titular, las ansiedades en las dudas que contesta y las frases literales como prueba (con permiso, como reseñas reales). Si usa `landing-que-convierte`, pásale el `.md`.
- **Formulario:** las opciones del primer paso, con las palabras de las ansiedades (`formulario-nepq`).
- **Repetirlo** cada pocos meses, o cuando entre un lote nuevo de reseñas: el lenguaje del cliente cambia.

## 8. Reglas

- **Nunca inventes citas ni cifras.** Toda cita es literal (con sus faltas, si las tiene) y lleva su ID. Todo recuento sale de contar el corpus. Si un dato no está, no está.
- **Separa siempre lo que dicen los clientes de tu interpretación**, en el informe y en la conversación.
- **Si hay menos de unas 15 reseñas con texto, dilo sin desanimar:** el análisis se hace igual, los recuentos son orientativos y conviene sumar otras fuentes. Avisa también si hay truncadas.
- **Privacidad:** ni nombres ni fotos de quien escribió la reseña. Si el cliente nombra a alguien del equipo del negocio (por ejemplo, a quien le atendió), se puede dejar.
- **Las reseñas negativas también cuentan:** son las mejores fuentes de ansiedades (en Home Server, los miedos salieron de sus 12 reseñas críticas o mixtas). No las quites para que el informe quede bonito.
- **Tono claro y directo**, en el idioma, la variante y el trato que eligió el negocio (España, Latinoamérica o voseo; tú, vos o usted).
- El pie de abajo es para quien lee la skill en GitHub. No lo repitas en la conversación.

## Fuentes del método

- El sistema de Kris Sugatan, explicado en un short de Ad World Prime (youtube.com/shorts/9bhffGQEr4Q): sacar reseñas de varias fuentes (Reddit, foros, la web de la competencia, Amazon), forzar tres preguntas (por qué compraron, qué temían cuando les llegaba el producto, qué les encantó después) y usarlo para producir 50 mensajes.
- La estructura del informe es la de los copy mining de Vibrana y Home Server que hicimos en Flowboost Marketing.

---

Método de **Diego** (@diego_flowboost), arquitecto de sistemas en **Flowboost Marketing**. Si quieres que te montemos el embudo entero, escríbeme **EQUIPO** por privado en Instagram.
