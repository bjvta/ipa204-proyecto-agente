# Proyecto integrador · Un agente que ve

**IPA 204 · Fundamentos de la IA y TIC · Universidad Nacional Ecológica · Periodo II/2026**

En parejas, van a construir un **agente que ve**: una página web que mira una foto con la cámara del celular, reconoce lo que ustedes le enseñaron y **decide qué hacer** con reglas de experto. Por ejemplo: «esta hoja de papa tiene plaga → aplicar control y revisar las plantas vecinas».

Lo distinto de este proyecto: **la IA la entrenan ustedes, con sus propias fotos**. Ninguna otra IA puede hacer eso por ustedes.

Lo publicarán gratis en **Hugging Face** para que cualquiera lo use desde su celular. No necesitan saber programar: para la página usarán **vibecoding**, pidiéndole a una IA (ChatGPT, Claude, Gemini u otra) que escriba el código.

## Así funciona su agente

| Parte | Qué hace | Cómo lo hacen | Clase |
| --- | --- | --- | --- |
| **Ojos** | Reconoce lo que hay en la foto | Entrenan un modelo con **sus fotos** en Teachable Machine | 5 · *machine learning* |
| **1 · Percibe** | Recibe la foto y otros datos | La cámara del celular es su sensor | 6 · sensores |
| **2 · Decide** | Aplica reglas «si… entonces» | Escriben reglas con lo que les dijo una persona experta | 4 y 10 · reglas de experto |
| **3 · Actúa** | Recomienda y explica por qué | La página muestra la recomendación | 1 · agentes |
| **4 · Registra** | Guarda cada consulta | Un historial descargable | 8 · trazabilidad |

## Un ejemplo a medias

[**Semáforo del plátano**](https://bjvta.github.io/ipa204-proyecto-agente/ejemplo/) ([código](ejemplo/index.html)): ábranlo, suban una de las [fotos de prueba](ejemplo/fotos/) y miren cómo reconoce si está verde, madura o pasada y qué recomienda. Está **incompleto a propósito** (solo 3 reglas) y usa un modelo sin entrenar. El suyo tendrá su propio modelo y mucho más.

La [plantilla](plantilla/index.html) es el punto de partida de su agente.

Ideas de problemas:

- **Agroecológica:** hojas sanas o con plaga (papa, haba, maíz), maleza o cultivo, grano de quinua limpio o con impurezas, madurez de frutos, estado del compost.
- **Alimentaria:** pan con moho o sin moho, defectos en frutas, color de papas fritas, envases bien o mal sellados, limpieza de una mesa de trabajo.

**Elijan un problema propio.** El plátano del ejemplo no se puede usar como proyecto.

## Calendario

| Hito | Fecha | Qué muestran en clase, antes de salir |
| --- | --- | --- |
| 1 · Lanzamiento | jueves 26/11 (clase 4) | Pareja, problema y qué verá su agente |
| 2 · Ficha y fotos | lunes 30/11 (clase 6) | [Ficha](guia/ficha-del-agente.md) completa y sus primeras fotos |
| 3 · Prototipo | jueves 03/12 (clase 9) | Modelo entrenado y su agente funcionando en Hugging Face |
| 4 · Pruebas | martes 08/12 (clase 12) | 10 fotos nuevas probadas, con aciertos y errores |
| 5 · Revisión ética | miércoles 09/12 (clase 13) | Privacidad, sesgo de sus fotos y límites |
| Ensayo general | viernes 11/12 (clase 15) | Muestran el agente y reciben comentarios |
| **Presentación final** | **lunes 14/12** | **7 minutos y demostración en vivo con el celular** |

**Los hitos no tienen nota:** son revisiones para que reciban comentarios a tiempo. **La nota del proyecto (30 puntos) se pone solo en la presentación final.** Los criterios están en la [rúbrica](rubrica.md).

## Paso a paso

1. [Crear las cuentas](guia/1-cuentas.md): Hugging Face y una IA para conversar.
2. [Completar la ficha del agente](guia/ficha-del-agente.md): qué ve, qué decide y de dónde salen sus reglas.
3. [Entrenar los ojos de su agente](guia/2-entrenar.md): sus fotos en Teachable Machine.
4. [Crear el agente con vibecoding](guia/3-vibecoding.md): instrucciones listas para copiar.
5. [Publicarlo en Hugging Face](guia/4-publicar.md): un Space estático, gratis.
6. [Probarlo](guia/5-pruebas.md): 10 fotos nuevas y qué hacer cuando falla.
7. [Revisión ética](guia/6-etica.md): privacidad, sesgo y límites.
8. [Presentación final](guia/7-presentacion.md): cómo mostrarlo en 7 minutos.

## Qué hay en este repositorio

```
plantilla/index.html     La plantilla del agente que ve: el punto de partida
ejemplo/                 Un agente de ejemplo, incompleto a propósito, con fotos de prueba
guia/                    El paso a paso
rubrica.md               Cómo se califica la presentación final
```

## Lo que se exige

1. **Sus propias fotos.** El modelo se entrena con fotos que toman ustedes, al menos 30 por clase, en su entorno real.
2. **Reglas con fuente.** Las reglas salen de una **entrevista** a alguien que trabaja en el tema o de una **fuente técnica concreta**. No valen valores inventados.
3. **Una regla difícil.** Al menos una regla combina lo que ve el modelo con otro dato (por ejemplo: «con plaga» **y** etapa de floración). Además, encuentran un caso donde dos reglas recomiendan cosas distintas y explican cuál debe ganar.
4. **Una mejora obligatoria.** Una de las [mejoras de la guía](guia/3-vibecoding.md#mejora-obligatoria): grados como en lógica difusa, un puntaje de riesgo con pesos o prioridad entre reglas.
5. **Defensa individual.** En la presentación, cada integrante explica una regla que elige el docente.

## Reglas del proyecto

- Trabajan en parejas.
- Pueden usar IA para escribir el código, pero **las fotos y las reglas son suyas**.
- Su agente **recomienda**: no reemplaza a una persona experta. Debe decirlo en pantalla.
