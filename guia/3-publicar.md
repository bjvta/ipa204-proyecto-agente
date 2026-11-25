# 3 · Publicarlo en Hugging Face

Van a crear un **Space estático**: una página web publicada en Hugging Face. Es gratis y no hay que instalar nada.

## Crear el Space

1. Entren a [huggingface.co/new-space](https://huggingface.co/new-space) con su cuenta.
2. Completen:
   - **Space name:** el nombre de su agente, sin espacios ni acentos. Ejemplo: `asesor-de-riego`.
   - **License:** pueden elegir `mit`.
   - **Space SDK:** elijan **Static**.
   - **Visibility:** **Public**, para que el docente y sus compañeros lo puedan abrir.
3. Pulsen **Create Space**.

Hugging Face crea el Space con un archivo `index.html` de ejemplo.

## Poner su agente

1. En su Space, entren a la pestaña **Files**.
2. Abran `index.html` y pulsen **Edit**.
3. Borren todo el contenido y peguen el código de su agente.
4. Abajo, pulsen **Commit changes to main** para guardar.

Otra opción: en **Files**, usen **Add file → Upload files** y suban su archivo `index.html` (debe llamarse exactamente así).

## Ver su agente

Vuelvan a la pestaña **App**. En unos segundos aparece su agente. El enlace para compartir es:

```
https://huggingface.co/spaces/SU-USUARIO/NOMBRE-DEL-SPACE
```

Ese es el enlace que entregan en el hito 3. Ábranlo también desde el celular para ver que se usa bien.

## Actualizarlo

Cada vez que mejoren el agente, repitan **Files → index.html → Edit → pegar → Commit**. El enlace no cambia.

## Si algo sale mal

| Problema | Qué hacer |
| --- | --- |
| La página sale en blanco | Pruébenla primero en su computadora (doble clic en el archivo). Si ahí también falla, el error está en el código: usen la instrucción de corrección de la [guía de vibecoding](2-vibecoding.md). |
| Se ve el ejemplo de Hugging Face y no su agente | Revisen que guardaron con **Commit** y que el archivo se llama `index.html`. Recarguen la página. |
| No encuentran la opción **Static** | Revisen que crearon un **Space** (no un modelo ni un dataset) desde [huggingface.co/new-space](https://huggingface.co/new-space). |
| Les pide pagar | Elijan **Static**. Las otras opciones (Gradio, Docker) necesitan un plan pago y no las usamos. |

## Listo cuando…

- [ ] El enlace de su Space abre su agente.
- [ ] Funciona desde una computadora y desde un celular.
- [ ] Muestra los nombres de los integrantes y sus límites.
