# norns canvas / U-MA

Editor de pantallas para el **monome norns** desde el celular: dibujás en la pantalla de 128×64 px con sus 16 niveles de brillo y exportás un script Lua listo para correr, o funciones para pegar en tu propio script.

**Abrir:** https://buenosairesfront.github.io/nornscanvas/
**Manual:** https://buenosairesfront.github.io/nornscanvas/docs/

Todo funciona en el navegador, sin instalar nada y sin cuenta. Los proyectos se guardan en el teléfono (almacenamiento local del navegador).

## Links para la landing de Instagram

| Link | Abre |
|---|---|
| `https://buenosairesfront.github.io/nornscanvas/` | el editor, en el último idioma usado (por defecto español) |
| `…/nornscanvas/?lang=en` | en inglés (`es`, `en`, `de`, `fr`, `ja`, `zh`, `hi`) |
| `…/nornscanvas/docs/` | el manual |

## Qué hace

- **Herramientas:** seleccionar, línea, lápiz, goma, balde, rectángulo (vacío / lleno), círculo (vacío / lleno), polígono y estrella (hasta 64 vértices), texto con las fuentes del norns.
- **Objetos y capas:** cada cosa que dibujás es un objeto editable. Capas con ocultar, bloquear y reordenar; grupos; selección múltiple.
- **Niveles:** 16 niveles de brillo (0–15), como el OLED del norns. Rellenos con patrón: 1 bit, tono Bayer, degradado tramado y generativos.
- **Librería:** más de 80 elementos listos — interfaz (botones, knobs, faders, VU, secuenciador de 16 pasos, pads, menús, teclado), señales (seno, cuadrada, sierra, ADSR, osciloscopio, espectro, Lissajous), íconos y formas.
- **Efectos:** invertir, brillo, 1 bit, dithering, posterizar, solarizar, ruido, degradados, tramados, scanlines, espejo, rotar, simetría, engrosar / adelgazar, pixelar, contorno, sombra, resplandor, eco y destellos.
- **Frames y animación:** varios frames con papel cebolla, fps del proyecto, y animación por objeto (oscilar, orbitar, rebotar, pulso de escala, fade…).
- **Imagen:** importar una foto y convertirla a 16 niveles con dithering.
- **Exportar:** script Lua completo o solo funciones, GIF animado, PNG del frame y hoja de sprites. Compartir como imagen o video con marco U-MA.
- **Botones del norns:** marcá un objeto como botón y el script exportado lo maneja con E2 (elegir) y K3 (presionar).

## Usarlo en el norns

1. Exportar → **Lua** → **Script completo** → Descargar (o Copiar código).
2. Copiá el archivo a `dust/code/<nombre>/<nombre>.lua` (por SMB, o pegalo en maiden).
3. Abrilo desde el menú SELECT del norns.

Para usar el dibujo dentro de un script tuyo, exportá **Funciones** y llamalas desde `redraw()` después de `screen.aa(0)`, `screen.line_width(1)`, `screen.line_cap("square")` y `screen.line_join("round")`.

## Archivos

- `index.html` — la aplicación entera (HTML + CSS + JS en un solo archivo).
- `docs/index.html` — manual de uso.

La IA de dibujo solo aparece cuando la herramienta se abre como artefacto dentro de claude.ai; en esta versión web queda oculta.

---

U-MA サウンド · Buenos Aires Front
