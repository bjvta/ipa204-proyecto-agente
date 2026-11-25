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

## Ejemplos para inspirarse

| Carrera | Ejemplo | Archivo |
| --- | --- | --- |
| Agroecológica y Desarrollo Rural Ambiental | Asesor de riego para la parcela | [`ejemplos/agroecologia-riego`](ejemplos/agroecologia-riego/index.html) |
| Producción e Innovación Alimentaria | Vigía de la cadena de frío | [`ejemplos/alimentos-cadena-de-frio`](ejemplos/alimentos-cadena-de-frio/index.html) |

Más ideas: diagnóstico de plagas por síntomas, guía de compostaje, calendario de siembra, control de secado de granos, asistente de un punto crítico HACCP, estimador de vida útil, revisión de etiquetas, control de fermentación de yogur.

**Elijan un problema propio.** No pueden entregar los ejemplos con otro nombre.

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
ejemplos/                Dos agentes de ejemplo, uno por carrera
guia/                    El paso a paso
rubrica.md               Cómo se califica cada hito
```

## Reglas del proyecto

- Trabajan en parejas. Los dos tienen que poder explicar cómo decide su agente.
- Pueden usar IA para escribir el código, pero **las reglas las deciden ustedes** y deben poder justificarlas con lo visto en clase o con una fuente.
- Si usan valores (temperaturas, porcentajes, tiempos), anoten de dónde salen.
- Su agente **recomienda**: no reemplaza a una persona experta. Debe decirlo en pantalla.
