# Eslàlom Gegant · Baqueira Beret 🎿

Pequeño videojuego HTML de **slalom gigante** de esquí alpino, hecho para que **Simón Kaibide** (#123, club **CEVA**) entrene la trazada y el ritmo de las puertas. Ambientado en el **Stadium Fernández Ochoa** de **Baqueira Beret**.

**▶ Jugar:** https://eslalom-simon.pages.dev

## Cómo se juega
- 30 puertas (parejas de banderas alternas **naranja / azul**), una cada ~2 s.
- **iPhone / iPad:** inclina el dispositivo para girar (hay que permitir el sensor de movimiento al empezar).
- **Ordenador:** flechas ⬅️ ➡️ (o A / D).
- **Táctil:** toca el lado izquierdo o derecho de la pantalla.
- 3 niveles — **Alevín / Infantil / Copa Europa**: a más nivel, puertas más estrechas y menos tiempo entre ellas.
- Cronómetro, % de puertas limpias, metrónomo de ritmo, velocímetro y récords.

## Técnico
- Un **único archivo** [`index.html`](index.html) — canvas 2D + JavaScript, **sin dependencias**. Funciona offline (doble clic).
- Motor **pseudo-3D** estilo *Alpine Racer / OutRun*: pista con curvas y relieve (cuestas).
- Datos del corredor (nombre, dorsal, club, país, color del traje) editables y guardados en el navegador.
- Desplegado en **Cloudflare Pages**.

## Desarrollo
Editar `index.html` y volver a publicar:

```bash
npx wrangler pages deploy . --project-name=eslalom-simon --branch=main --commit-dirty=true
```

## Logos

Los logotipos van en `assets/` (`baqueira.png`, `ceva.png`). No se incluyen en el
repositorio; si faltan, el juego muestra texto en su lugar.

## Créditos y licencia

Proyecto **familiar, sin ánimo de lucro**.

- **Código**: Creative Commons **CC BY-NC 4.0** (uso/adaptación no comercial citando autoría). Ver [`LICENSE`](LICENSE).
- **Marcas**: *Baqueira Beret* (Baqueira/Beret, S.A.) y *CEVA* (Club d'Esquí Vall d'Aran) son
  propiedad de sus titulares; se usan solo con fin identificativo en un proyecto privado y
  **no están** bajo la licencia CC. Se retirarán a petición de sus propietarios.

Hecho con cariño (y con Claude Code).
