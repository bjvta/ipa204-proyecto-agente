# 5 · Probar el agente (hito 4)

Un agente que no se prueba no es confiable. En la clase 5 vimos que un modelo se evalúa con **datos que nunca vio**. Aquí usarán las 10 fotos que guardaron aparte al entrenar.

## Qué entregan

Una tabla con **10 fotos nuevas**, que el modelo no vio al entrenar. Para cada foto:

1. Anoten qué hay realmente en la foto (la clase correcta) y los datos extra.
2. Antes de probar, anoten **qué debería responder** el agente (según su ficha).
3. Pruébenlo y anoten **qué vio el modelo, con qué confianza, y qué recomendó**.
4. Marquen si acertó.

| # | Qué hay en la foto | Qué debería responder | Qué vio el modelo (confianza) | Qué recomendó | ¿Acertó? |
| --- | --- | --- | --- | --- | --- |
| 1 | | | | | |
| 2 | | | | | |
| … | | | | | |
| 10 | | | | | |

**Aciertos:** ___ de 10 · **Exactitud:** aciertos ÷ 10 = ___ %

## Qué casos elegir

No prueben solo casos fáciles. Incluyan:

- **Fotos normales** de cada clase.
- **Fotos difíciles:** otra luz, otro fondo, de lejos, un ejemplar raro.
- **Una foto de «otra cosa»** que no es ninguna clase. ¿El agente dice que no está seguro?
- **Un caso límite** de una regla: por ejemplo, una foto donde el modelo duda (cerca de 60 % de confianza).
- **El choque de su ficha:** el caso donde dos reglas recomiendan cosas distintas. ¿Gana la que debe ganar?

## Si falla

Para cada caso donde no acertó, escriban:

- ¿Por qué falló? ¿El modelo vio mal (faltaban fotos parecidas al entrenar) o la regla estaba mal?
- ¿Qué cambiaron para corregirlo?

Corregir errores **suma**: muestra que entendieron cómo decide su agente.

## Listo cuando…

- [ ] Tienen 10 fotos nuevas, con fotos difíciles y una de «otra cosa».
- [ ] Cada caso tiene la respuesta esperada **antes** de probar.
- [ ] Explican cada error y qué cambiaron.
- [ ] Si reentrenaron el modelo o cambiaron reglas, publicaron la versión corregida.
