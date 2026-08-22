# fluxbound-web

Landing page de [Fluxbound](https://github.com/xavierbasc/fluxbound).

Sitio estático, sin paso de compilación: es HTML y CSS en un fichero, y por eso
no puede romperse en un despliegue. GitHub Pages lo sirve tal cual.

El contenido vive en el repo del juego, en `web/`, y se publica con:

```bash
git subtree push --prefix=web git@github.com:xavierbasc/fluxbound-web.git main
```

En GitHub: Settings → Pages → Source: `main` / `root`.

Las capturas de `shots/` se regeneran con el propio juego:

```bash
cd dist/macos && ./Fluxbound.app/Contents/MacOS/Fluxbound --screenshot
```
