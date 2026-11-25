# 2 · Crear el agente con vibecoding

**Vibecoding** es construir un programa conversando con una IA: ustedes dicen qué quieren, la IA escribe el código, ustedes lo prueban y piden cambios.

Para que salga bien, partimos de una **plantilla** que ya funciona. Ustedes solo cambian el bloque marcado como `EDITA DESDE AQUÍ`.

## Paso 1 · Copien la plantilla

1. Abran [`plantilla/index.html`](../plantilla/index.html) y pulsen el botón **Raw** (o «Copy raw file»).
2. Copien todo el texto.

## Paso 2 · Pídanle a la IA su agente

Copien esta instrucción en la IA. Reemplacen lo que está entre corchetes y peguen al final la plantilla y su ficha.

```text
Eres un asistente que ayuda a estudiantes de 2.º semestre a construir un agente sencillo.

Te paso una plantilla HTML que ya funciona. Solo debes cambiar el bloque que está entre
«EDITA DESDE AQUÍ» y «HASTA AQUÍ». No cambies nada más del archivo.

Mi agente se llama: [nombre]
Integrantes: [nombres]
Carrera: [carrera]
Resuelve este problema: [2 líneas]

Datos de entrada (percibe):
[pega aquí la tabla de datos de tu ficha]

Reglas (decide):
[pega aquí la tabla de reglas de tu ficha]

Si no se cumple ninguna regla, el agente dice: [texto]
Límites del agente: [texto]

Devuélveme el archivo index.html COMPLETO, listo para copiar.
Escribe todo en español. Cada regla debe tener su «porque» en palabras sencillas.

Esta es la plantilla:
[pega aquí todo el texto de plantilla/index.html]
```

## Paso 3 · Pruébenlo en su computadora

1. Copien el código que les dio la IA.
2. Abran el **Bloc de notas** (Windows) o **TextEdit** en modo texto plano (Mac), peguen y guarden como `index.html`.
3. Hagan doble clic en el archivo: se abre en el navegador.
4. Completen el formulario y pulsen **Consultar al agente**.

¿Funciona? Pasen a [publicarlo](3-publicar.md). ¿No funciona? Usen las instrucciones de abajo.

## Instrucciones para corregir y mejorar

Copien la que necesiten en la **misma conversación**.

**La página sale en blanco o el botón no hace nada**

```text
La página no funciona: [describe qué pasa]. Revisa el bloque EDITA DESDE AQUÍ,
busca errores de sintaxis (comas, comillas, llaves) y devuélveme el archivo completo corregido.
```

**Una regla no se activa cuando debería**

```text
Con estos datos: [valores], esperaba que el agente dijera «[acción]», pero dijo «[lo que dijo]».
Explícame por qué y corrige la regla. Devuélveme el archivo completo.
```

**Agregar o cambiar una regla**

```text
Agrega esta regla: si [condición], entonces [acción], con nivel [ok/aviso/alerta],
porque [razón]. Devuélveme el archivo completo.
```

**Agregar un dato de entrada**

```text
Agrega este dato de entrada: [nombre], de tipo [número/opciones], con [valores o rango] y
unidad [unidad]. Úsalo en esta regla: [regla]. Devuélveme el archivo completo.
```

**Entender el código (para la presentación)**

```text
Explícame en palabras sencillas, como para un estudiante de 2.º semestre, cómo decide
mi agente: qué hace cada regla y en qué orden se revisan.
```

## Mejora obligatoria

Su agente tiene que incluir **una** de estas tres mejoras. Vale 2 puntos en la presentación final. Agréguenla **después** de que el agente básico funcione.

### Opción A · Grados, como en lógica difusa (clase 4)

En lugar de decir solo «hace calor» o «no hace calor», el agente calcula **cuánto** (un grado entre 0 y 1) y lo muestra.

```text
Quiero que mi agente use grados como en lógica difusa. Para el dato [nombre del dato],
el conjunto «[alto, caliente, seco…]» vale 0 en [valor] y 1 en [valor], subiendo en línea recta.
Calcula ese grado dentro de las reglas y muéstralo en el «porque», por ejemplo:
«Grado de caliente: 0,75». Usa la regla con nivel alerta si el grado es mayor que [valor]
y aviso si está entre [valor] y [valor]. Cambia solo el bloque EDITA DESDE AQUÍ.
Devuélveme el archivo completo.
```

### Opción B · Puntaje de riesgo con pesos (clase 5)

Como una neurona artificial: cada dato suma o resta según su **peso**, y el total decide.

```text
Quiero que mi agente calcule un puntaje de riesgo, como una neurona artificial.
Datos y pesos: [dato 1] con peso [número], [dato 2] con peso [número], [dato 3] con peso [número].
Antes, convierte cada dato a una escala de 0 a 1 así: [explica cómo].
Si el puntaje supera [umbral], recomienda «[acción]» con nivel alerta. Muestra el puntaje
en el «porque». Cambia solo el bloque EDITA DESDE AQUÍ. Devuélveme el archivo completo.
```

### Opción C · Prioridad entre reglas (sistema experto, clases 4 y 10)

Cuando dos reglas chocan, una debe ganar. Usen el choque que describieron en su ficha.

```text
En mi agente, la regla «[regla que debe ganar]» tiene prioridad: si se cumple, el agente no
debe revisar las demás reglas. Ponla primera en la lista y agrégale detener: true.
Explícame en el «porque» por qué tiene prioridad. Cambia solo el bloque EDITA DESDE AQUÍ.
Devuélveme el archivo completo.
```

Para la presentación deben poder explicar su mejora **con sus palabras**: qué calcula, con qué números y por qué la eligieron.

## Buenas prácticas

- Guarden **cada versión que funcione** con otro nombre (`index-v1.html`, `index-v2.html`). Si algo se rompe, vuelven a la anterior.
- Pidan **un cambio a la vez**. Si piden diez cosas juntas, es difícil saber qué falló.
- Lean el bloque `EDITA DESDE AQUÍ`: ahí están sus reglas en un lenguaje casi como el español.
