# Skills de Claude para embudos que venden

Cinco skills para Claude Code con el método que uso en **Flowboost Marketing** para que los anuncios traigan clientes y no solo leads. Funcionan en tu ordenador, dentro de Claude Code: sin cuentas ni herramientas externas.

| Skill | Qué hace | Qué te deja en la carpeta |
|---|---|---|
| [`revisor-de-embudo`](revisor-de-embudo/) | Revisa tu embudo entero con los 6 puntos: **anuncios → landing → VSL → formulario → página de gracias → llamada en 5 minutos**. Te dice qué está bien y qué cambiar, por orden de impacto | La revisión, en la conversación |
| [`brief-de-oferta`](brief-de-oferta/) | Claude te entrevista, pregunta por pregunta, para sacar el brief de tu oferta antes de construir nada. Guarda un borrador por bloques, así que puedes parar y seguir | `brief.md` |
| [`landing-que-convierte`](landing-que-convierte/) | Del brief al texto y del texto a una landing en un solo HTML, rápida, móvil primero y con una sola acción | `landing-texto.md` · `index.html` · `pendientes.md` |
| [`formulario-nepq`](formulario-nepq/) | El formulario de varios pasos que cualifica: primero el objetivo y el dolor, y los datos al final. Te lo da en texto, para cualquier herramienta | `formulario-nepq.md` |
| [`pagina-de-gracias`](pagina-de-gracias/) | La página de gracias que hace que el lead espere tu llamada: quién llama, cuándo, desde qué número y de qué se habla | `gracias.html` |

**El orden recomendado:** `brief-de-oferta` → `landing-que-convierte` → `formulario-nepq` → `pagina-de-gracias`. Y cuando ya tengas anuncios funcionando, `revisor-de-embudo`.

## Instalación

**En Claude Code** (todas las skills, para todos tus proyectos):

```bash
git clone https://github.com/diegogwork1-alt/embudos-que-venden.git
mkdir -p ~/.claude/skills
cd embudos-que-venden && cp -r revisor-de-embudo brief-de-oferta landing-que-convierte formulario-nepq pagina-de-gracias ~/.claude/skills/
```

Si solo las quieres en un proyecto, cópialas en la carpeta `.claude/skills/` de ese proyecto.

**Cómo se usan:** abre Claude Code en la carpeta de tu proyecto y pídelo con tus palabras. Claude elige la skill:
- «Revisa mi embudo, esta es mi landing: https://…»
- «Hazme el brief de mi negocio»
- «Quiero una landing para mi clínica»
- «Rehazme el formulario, solo pido nombre y teléfono»
- «Hazme la página de gracias»

## El método, en una frase

Un lead no es un cliente. La venta se gana o se pierde en lo que pasa después del clic: una landing que explica, un vídeo que calienta, un formulario que filtra, una página de gracias que prepara la llamada y una llamada en los primeros 5 minutos.

---

Hecho por **Diego** · [@diego_flowboost](https://instagram.com/diego_flowboost) · arquitecto de sistemas en [Flowboost Marketing](https://flowboostmarketing.com).
Si prefieres que te montemos el embudo entero, escríbeme **EQUIPO** por privado en Instagram.
