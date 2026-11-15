# Monster Sim: Aotearoa 🦖🇳🇿

Simulador de defensa civil de kaijus en Nueva Zelanda. Un solo archivo (`index.html`), sin instalar nada: HTML + JavaScript + canvas.

*A single-file NZ Civil Defence kaiju simulation. Open `index.html` in a browser to play.*

https://crisai2026.github.io/monster-sim-aotearoa/

## Cómo jugar

1. Abre `index.html` en Chrome o Safari (doble clic).
2. Elige una ciudad y un monstruo, ajusta el tiempo de aviso de evacuación.
3. Pulsa **Start Simulation** y usa los puntos de acción (AP) para colocar defensas haciendo clic en el mapa:
   - 🎯 Artillería: dispara al monstruo más cercano
   - 🚒 FENZ: apaga fuegos en 2 celdas
   - 🚁 Chopper: evacúa más rápido en ~4 celdas
   - 🧱 Seawall: frena la marea de Abismo y reduce daños

## Cómo agregar el video del trailer

El juego busca un archivo llamado **`trailer.mp4`** en la misma carpeta que `index.html`.

1. Entra al repo en GitHub y pulsa **Add file → Upload files**.
2. Arrastra tu video. **El nombre debe ser exactamente `trailer.mp4`** (en minúsculas).
3. Pulsa **Commit changes**.

Notas:
- Por el navegador, GitHub acepta archivos de hasta **25 MB**. Si tu video pesa más, comprímelo (por ejemplo con HandBrake) o súbelo con `git`, que acepta hasta 100 MB.
- Formato recomendado: MP4 con H.264.
- Si solo quieres probarlo en tu computador, no hace falta subirlo: usa el botón **Load Alternative Video File** de la pantalla de inicio.

## Publicarlo en la web (GitHub Pages)

1. En el repo: **Settings → Pages**.
2. En *Build and deployment*, elige **Deploy from a branch**, rama **main**, carpeta **/ (root)**, y guarda.
3. En uno o dos minutos el juego queda en `https://crisai2026.github.io/monster-sim-aotearoa/`.

## Ajustes rápidos (en `index.html`)

- `MONSTER_SCALE`: tamaño de los monstruos en el mapa (0.6 por defecto).
- Tabla `MONS`: vida, velocidad, poder y blindaje de cada monstruo.
- Tabla `CITIES`: población, resistencia de edificios y rutas de evacuación.

## Sonido

Todo el audio (efectos y música) se genera con código, no hay archivos de sonido. Los botones **Music** y **Sound** de la barra superior los apagan por separado.
