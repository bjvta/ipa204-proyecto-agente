# 2 · Entrenar los ojos de su agente

Su agente va a **mirar fotos** y reconocer lo que ustedes le enseñen: una hoja sana o con plaga, un pan con moho o sin moho, un grano limpio o con impurezas. Para eso van a entrenar un modelo de IA con **sus propias fotos**, en [Teachable Machine](https://teachablemachine.withgoogle.com), una herramienta gratuita de Google que funciona en el navegador.

Es lo mismo que practicamos en el laboratorio de la clase 5 con el lapicero y el cuaderno: el modelo aprende de ejemplos con su etiqueta.

## Paso 1 · Decidan las clases

Una **clase** es cada cosa que el modelo debe distinguir. Elijan **entre 2 y 4**.

| Problema | Clases posibles |
| --- | --- |
| Plagas en hojas de papa | Sana · Con plaga · Seca |
| Moho en el pan | Sin moho · Con moho |
| Limpieza de quinua | Limpia · Con piedritas · Con cáscara |
| Madurez de tomates | Verde · Pintón · Maduro |

Consejos:

- Las clases deben **verse distintas en una foto**. «Rico» o «caro» no se ven; «con manchas» sí.
- Agreguen una clase **«Otra cosa»** con fotos de fondo, manos o mesa vacía. Así el agente no inventa una respuesta cuando no hay nada.

## Paso 2 · Tomen las fotos

Es la parte más importante. **Un modelo es tan bueno como sus fotos.**

- **Al menos 30 fotos por clase.** Mejor 50.
- **Fotos variadas:** distinta luz (sol, sombra, interior), distintos fondos, de cerca y de lejos, distintos ejemplares.
- **Fotos reales** de su entorno: el campo, el mercado, su casa, una planta. No bajen fotos de internet.
- **Guarden 10 fotos aparte** que el modelo **nunca** verá al entrenar. Las usarán para probarlo (hito 4).

Anoten dónde y cuándo tomaron las fotos: lo van a necesitar para la revisión ética.

## Paso 3 · Entrenen el modelo

1. Entren a [teachablemachine.withgoogle.com](https://teachablemachine.withgoogle.com) y pulsen **Comenzar** (*Get Started*).
2. Elijan **Proyecto de imagen** (*Image Project*) → **Modelo de imagen estándar**.
3. Cambien el nombre de cada **clase** (*Class 1*, *Class 2*…) por los nombres que eligieron. Escríbanlos con cuidado: los usarán en sus reglas.
4. En cada clase, pulsen **Subir** (*Upload*) y suban sus fotos. También pueden usar la **cámara** (*Webcam*): mantengan apretado el botón de grabar mientras mueven el objeto.
5. Pulsen **Entrenar modelo** (*Train Model*) y esperen. **No cambien de pestaña**: si lo hacen, el entrenamiento se pausa.
6. **Pruébenlo** en el panel de la derecha (*Vista previa*) con la cámara o con una foto nueva. Las barras muestran qué tan seguro está.

¿Se equivoca mucho? Agreguen fotos **distintas** (otra luz, otro fondo, otra posición) a la clase que confunde y vuelvan a pulsar **Entrenar modelo**. Las fotos nuevas se suman a las anteriores. Para borrar una foto mala, pasen el mouse sobre ella y usen el ícono de basura.

Para ver cuánto acierta cada clase: **Avanzado** → **Detalles internos** (*Under the hood*).

## Paso 4 · Exporten el enlace

1. Pulsen **Exportar modelo** (*Export Model*).
2. Elijan la pestaña **Tensorflow.js** y la opción **Subir (enlace para compartir)** (*Upload (shareable link)*).
3. Pulsen **Subir mi modelo** (*Upload my model*).
4. Copien el enlace que aparece. Se ve así:

```
https://teachablemachine.withgoogle.com/models/AbCdEf123/
```

Ese enlace son los «ojos» de su agente. Lo pegarán en la plantilla (paso siguiente).

**Guarden también el proyecto** (menú ☰ → *Guardar proyecto en Drive*) para poder agregar fotos y volver a entrenar después. Cada vez que reentrenen, usen **Actualizar mi modelo en la nube** y el enlace sigue siendo el mismo.

## Plan B: sin entrenar

Si no logran juntar fotos suficientes, la plantilla también funciona con un modelo de Hugging Face (CLIP) que compara la foto con descripciones escritas en inglés, sin entrenar. Es el que usa el [ejemplo](../ejemplo/index.html). Consulten antes con el docente: el plan A (sus propias fotos) es lo que se espera del proyecto.

## Listo cuando…

- [ ] Tienen entre 2 y 4 clases que se distinguen en una foto.
- [ ] Tienen al menos 30 fotos variadas por clase, tomadas por ustedes.
- [ ] Guardaron 10 fotos aparte para las pruebas.
- [ ] El modelo está entrenado y tienen su enlace.
