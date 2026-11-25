# 4 · Probar el agente (hito 4)

Un agente que no se prueba no es confiable. En la clase 5 vimos que un modelo se evalúa con casos que no conoce. Aquí harán lo mismo con sus reglas.

## Qué entregan

Una tabla con **10 casos**. Para cada caso:

1. Escriban los datos de entrada.
2. Antes de probar, anoten **qué debería responder** el agente (según su ficha).
3. Pruébenlo y anoten **qué respondió**.
4. Marquen si acertó.

| # | Datos de entrada | Qué debería responder | Qué respondió | ¿Acertó? |
| --- | --- | --- | --- | --- |
| 1 | | | | |
| 2 | | | | |
| … | | | | |
| 10 | | | | |

**Aciertos:** ___ de 10

## Qué casos elegir

No prueben solo casos fáciles. Incluyan:

- **Casos normales**, donde todo está bien.
- **Casos límite**, justo en el borde de una regla: si la regla dice «más de 30», prueben con 30 y con 31.
- **Casos raros** pero posibles: valores muy altos o muy bajos, combinaciones poco comunes.
- **Un caso donde se activen dos reglas a la vez.** ¿Las recomendaciones se contradicen?

## Si falla

Para cada caso donde no acertó, escriban:

- ¿Por qué falló? (una regla mal escrita, un límite mal puesto, un caso que nadie previó)
- ¿Qué cambiaron para corregirlo?

Corregir errores **suma**: muestra que entendieron cómo decide su agente.

## Listo cuando…

- [ ] Tienen 10 casos, con al menos 2 casos límite.
- [ ] Cada caso tiene la respuesta esperada **antes** de probar.
- [ ] Explican cada error y qué cambiaron.
- [ ] Publicaron la versión corregida en su Space.
