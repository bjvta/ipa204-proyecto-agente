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

## Nivel avanzado (opcional)

Si les sobra tiempo, pueden pedirle a la IA alguna de estas mejoras. Pruébenlas bien: una mejora que rompe el agente resta, no suma.

- **Grados como en lógica difusa** (clase 4): que el agente diga «riesgo alto en grado 0,7» en lugar de solo sí o no.
- **Un gráfico** del historial de consultas.
- **Varias reglas combinadas** con «y» y «o».

## Buenas prácticas

- Guarden **cada versión que funcione** con otro nombre (`index-v1.html`, `index-v2.html`). Si algo se rompe, vuelven a la anterior.
- Pidan **un cambio a la vez**. Si piden diez cosas juntas, es difícil saber qué falló.
- Lean el bloque `EDITA DESDE AQUÍ`: ahí están sus reglas en un lenguaje casi como el español.
