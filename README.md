# Proyecto integrador · Tu propio agente de IA

**IPA 204 · Fundamentos de la IA y TIC · Universidad Nacional Ecológica · Periodo II/2026**

En parejas, van a construir un **agente**: una página web que **percibe** datos, **decide** con reglas de experto y **actúa** con una recomendación que explica por qué. Lo publicarán gratis en **Hugging Face** para que cualquiera lo pueda usar desde su celular.

No necesitan saber programar. Usarán **vibecoding**: le piden a una IA (ChatGPT, Claude, Gemini u otra) que escriba el código con instrucciones claras, lo prueban y lo corrigen.

## Así funciona un agente

| Parte | Qué hace | En tu página |
| --- | --- | --- |
| **1 · Percibe** | Recibe datos del entorno | Un formulario: temperatura, humedad, producto, etapa… |
| **2 · Decide** | Aplica reglas «si… entonces» | Las reglas que escriben ustedes con lo visto en clase |
| **3 · Actúa** | Hace o recomienda algo | Una recomendación con su «por qué» |
| **4 · Registra** | Guarda lo que pasó | Un historial que se puede descargar |

Es el mismo agente de la clase 1, con las reglas de experto de las clases 4 y 10.

## Un ejemplo a medias

[**Vigía de la cadena de frío**](https://bjvta.github.io/ipa204-proyecto-agente/ejemplo/) ([código](ejemplo/index.html)): ábranlo y pruébenlo para ver cómo funciona un agente. Está **incompleto a propósito**: tiene solo 2 reglas y valores ilustrativos. El suyo tiene que ser mucho más que esto.

La [plantilla](https://bjvta.github.io/ipa204-proyecto-agente/plantilla/) es el punto de partida de su agente.

Ideas de problemas: riego de una parcela, diagnóstico de plagas por síntomas, compostaje, calendario de siembra, secado de granos, un punto crítico HACCP, vida útil de un producto, fermentación de yogur, recepción de leche cruda.

**Elijan un problema propio.** La cadena de frío del ejemplo no se puede usar como proyecto.

## Calendario

| Hito | Fecha | Qué entregan | Puntos |
| --- | --- | --- | --- |
| 1 · Lanzamiento | jueves 26/11 (clase 4) | Pareja y problema elegido | 2 |
| 2 · Ficha del agente | lunes 30/11 (clase 6) | [Ficha](guia/ficha-del-agente.md) completa | 4 |
| 3 · Prototipo | jueves 03/12 (clase 9) | Enlace a su agente funcionando en Hugging Face | 6 |
| 4 · Pruebas | martes 08/12 (clase 12) | 10 casos probados, con aciertos y errores | 5 |
| 5 · Revisión ética | miércoles 09/12 (clase 13) | Privacidad, sesgo y límites de su agente | 3 |
| Ensayo general | viernes 11/12 (clase 15) | Muestran el agente y reciben comentarios | — |
| 6 · Presentación final | lunes 14/12 | Presentación de 7 minutos y demostración en vivo | 10 |
| | | **Total** | **30** |

Los criterios de cada hito están en la [rúbrica](rubrica.md).

## Paso a paso

1. [Crear las cuentas](guia/1-cuentas.md): Hugging Face y una IA para conversar.
2. [Completar la ficha del agente](guia/ficha-del-agente.md): qué percibe, qué decide y qué hace.
3. [Crear el agente con vibecoding](guia/2-vibecoding.md): instrucciones listas para copiar.
4. [Publicarlo en Hugging Face](guia/3-publicar.md): un Space estático, gratis.
5. [Probarlo](guia/4-pruebas.md): 10 casos y qué hacer cuando falla.
6. [Revisión ética](guia/5-etica.md): privacidad, sesgo y límites.
7. [Presentación final](guia/6-presentacion.md): cómo mostrarlo en 7 minutos.

## Qué hay en este repositorio

```
plantilla/index.html     La plantilla del agente: el punto de partida
ejemplo/                 Un agente de ejemplo, incompleto a propósito
guia/                    El paso a paso
rubrica.md               Cómo se califica cada hito
```

## Lo que se exige

1. **Datos del mundo real.** Sus reglas salen de una **entrevista** a alguien que trabaja en el tema (un productor, una persona de planta, un técnico) o de una **fuente técnica concreta** (un manual, una norma, un artículo). Lo anotan en la ficha. No valen valores inventados.
2. **Una regla difícil.** Al menos una regla combina dos datos (por ejemplo, humedad **y** etapa del cultivo). Además, encuentran un caso donde dos reglas recomiendan cosas distintas y explican cuál debe ganar.
3. **Una mejora obligatoria.** Su agente incluye una de las [mejoras de la guía](guia/2-vibecoding.md#mejora-obligatoria): grados como en lógica difusa, un puntaje de riesgo con pesos o prioridad entre reglas.
4. **Defensa individual.** En la presentación, cada integrante explica una regla que elige el docente. Los dos tienen que entender todo el agente.

## Reglas del proyecto

- Trabajan en parejas.
- Pueden usar IA para escribir el código, pero **las reglas las deciden ustedes** con su entrevista o su fuente.
- Su agente **recomienda**: no reemplaza a una persona experta. Debe decirlo en pantalla.
