# Ficha del agente (hito 2)

Copien esta ficha en un documento o en papel, complétenla y tráiganla a la clase del lunes 30/11 junto con sus primeras fotos (al menos 10 por clase): se entrega en clase, antes de salir. Es el plano de su agente: la IA lo va a construir a partir de esta ficha.

---

**Nombre del agente:**

**Integrantes:**

**Carrera:**

## 1. El problema

- ¿Qué problema resuelve? (2 o 3 líneas)
- ¿Quién lo usaría? (un productor, una operaria de planta, un técnico…)
- ¿Qué pasa hoy sin el agente?

## 2. La fuente: de dónde sale el saber de su agente

Un sistema experto guarda el saber de una persona experta (clase 4). Elijan **una** de estas dos opciones.

**Opción A · Entrevista** (recomendada)

Conversen 15 minutos con alguien que trabaje en el tema: un productor, una persona de una planta o de un laboratorio, un técnico agrícola, una persona de su familia que lo haga todos los días.

- Nombre (o iniciales) y a qué se dedica:
- Fecha y forma (en persona, llamada, mensajes):

Preguntas guía:

1. ¿Qué decisión toma usted seguido sobre [el tema]?
2. ¿En qué se fija para decidir? ¿Qué mide o qué mira?
3. ¿A partir de qué valor cambia lo que hace? («si pasa de…, entonces…»)
4. ¿Qué errores son los más comunes? ¿Qué pasa cuando alguien se equivoca?
5. ¿Hay casos donde la regla de siempre no sirve?

Resumen de lo que respondió (5 a 8 líneas):

**Opción B · Fuente técnica**

Un manual, una norma, una guía de una institución o un artículo. Anoten el título, el autor o la institución, el año y el enlace o la página. Copien los valores que usarán.

## 3. Percibe: qué ve y qué más pregunta

**Las clases que verá el modelo** (entre 2 y 4, más «Otra cosa»):

| Clase | Cómo se ve en una foto | Dónde tomarán las fotos |
| --- | --- | --- |
| Ejemplo: Con plaga | Hojas con agujeros o manchas cafés | Parcela de la familia, en Achocalla |
| | | |
| | | |
| Otra cosa | Fondo, manos, tierra sin hojas | Los mismos lugares |

**Plan de fotos:** ¿cuántas fotos por clase (al menos 30)? ¿Con qué luz y fondos distintos? ¿Cuándo las tomarán?

**Datos extra** (de 0 a 3) que el agente pedirá además de la foto:

| Dato | Tipo | Valores posibles | Unidad |
| --- | --- | --- | --- |
| Ejemplo: etapa del cultivo | opciones | siembra, crecimiento, floración | — |
| | | | |

## 4. Decide: las reglas

Entre 4 y 8 reglas «si… entonces». Pueden usar lo que ve el modelo (la clase y qué tan seguro está) y los datos extra. Cada valor tiene que salir de su fuente.

| # | Si… (condición) | Entonces… (acción) | Nivel | Por qué | Fuente |
| --- | --- | --- | --- | --- | --- |
| 1 | Ejemplo: el modelo ve «Con plaga» con más de 70 % de seguridad **y** la etapa es floración | Aplicar control hoy y revisar las plantas vecinas | alerta | En floración la plaga daña más la cosecha | Entrevista a don J. M., productor |
| 2 | Ejemplo: el modelo está menos de 60 % seguro | Tomar otra foto con mejor luz | aviso | No conviene decidir con una foto dudosa | Recomendación de la guía |
| 3 | | | | | |
| 4 | | | | | |

Niveles: **ok** (todo bien), **aviso** (atención) o **alerta** (actuar ya).

- **La regla difícil:** ¿cuál de sus reglas combina lo que ve el modelo con otro dato? (número de regla)
- **El choque:** describan un caso en el que dos reglas recomienden cosas distintas. ¿Cuál debe ganar y por qué?
- ¿Qué dice el agente si **ninguna** regla se cumple?

## 5. Actúa: qué hace

- ¿Qué recomendaciones da?
- ¿Qué **no** hace o no sabe? (sus límites)

## 6. La mejora que van a agregar

Elijan una de la [guía de vibecoding](3-vibecoding.md#mejora-obligatoria) y expliquen en 2 líneas cómo la usarán en su agente.

---

## Listo cuando…

- [ ] El problema es concreto y de su carrera.
- [ ] Tiene una entrevista resumida o una fuente técnica completa.
- [ ] Tiene entre 2 y 4 clases que se distinguen en una foto, y un plan de fotos.
- [ ] Tiene entre 4 y 8 reglas, cada una con su «por qué» y su fuente.
- [ ] Una regla combina lo que ve el modelo con otro dato, y describe un choque entre reglas.
- [ ] Eligió la mejora obligatoria.
