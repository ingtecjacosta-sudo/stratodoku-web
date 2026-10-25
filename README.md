# Stratodoku web

Versión web del juego [Stratodoku](https://github.com/ingtecjacosta-sudo/Stratodoku) para jugar en **iPhone** (o cualquier navegador).

**Jugar:** https://ingtecjacosta-sudo.github.io/stratodoku-web/

## Instalar en el iPhone

1. Abre el enlace en **Safari**.
2. Toca el botón **Compartir** (el cuadrado con la flecha hacia arriba).
3. Elige **Agregar a pantalla de inicio** → **Agregar**.

Queda un icono de Stratodoku que abre el juego a pantalla completa, como una app. Funciona sin internet
después de abrirlo una vez. En Android con Chrome: menú ⋮ → **Instalar app**.

## Qué incluye

Lo mismo que la app de Android: 4 dificultades con tableros de solución única, notas, 3 pistas,
deshacer, límite de 3 errores, cronómetro con pausa, guardado automático y récords (10 mejores tiempos
por dificultad) con nombre y avatar (emoji o foto). Efectos al completar un cuadro (salto verde, sin mensaje) y al completar el Sudoku (ola naranja y confeti). En computadora también se juega con el teclado:
números, flechas y Borrar.

La partida y los récords propios se guardan en el navegador. Además hay una **tabla mundial** (Firebase), compartida con la app de Android: los récords se suben al guardarlos y, sin internet, quedan pendientes hasta que vuelva la conexión. En la tabla mundial los avatares son solo emojis.

## Archivos

| Archivo | Para qué |
|---|---|
| `index.html` | Todo el juego (diseño y lógica) |
| `manifest.webmanifest` | Nombre, colores e iconos al agregarla a la pantalla de inicio |
| `sw.js` | Permite usarla sin internet. Al publicar cambios, sube el número de `VERSION` aquí y `APP_VERSION` en `index.html` |
| `icons/` | Iconos de la app |

Se publica con GitHub Pages desde la rama `gh-pages`: al subir un cambio a `main`, súbelo también a `gh-pages` (`git push origin main:gh-pages`).
