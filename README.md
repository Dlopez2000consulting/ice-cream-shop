# Ice Cream Shop — 3D Gaussian Splat Web Viewer

## ⚠️ Paso que falta antes de subir a GitHub

### 1. Obtener el archivo `scene.compressed.ply`

Ve a **[SuperSplat](https://supersplat.playcanvas.com)**:

1. Arrastra tu `Ice_Cream_Shop.ply` a la ventana
2. Ajusta la cámara a la posición inicial que quieras
3. Ve a **File → Export → Compressed PLY** (o Export Scene)
4. Descarga el `.zip` exportado
5. Dentro del zip habrá un `scene.compressed.ply` → **reemplaza el de esta carpeta `docs/`**

> 💡 SuperSplat comprime el PLY de ~557MB a unos 50-100MB aprox.

### 2. (Opcional) Actualizar settings.json

Si en SuperSplat ajustaste la cámara y exportaste también el `settings.json`, reemplaza el de `docs/` con ese.

### 3. Subir a GitHub Pages

```bash
git init
git add .
git commit -m "Ice Cream Shop 3DGS viewer"
git branch -M main
git remote add origin https://github.com/TU_USUARIO/ice-cream-shop-3dgs.git
git push -u origin main
```

Luego en GitHub:
- Settings → Pages → Source: **Deploy from branch `main`, folder `/docs`**
- Tu escena estará en: `https://TU_USUARIO.github.io/ice-cream-shop-3dgs/`

## Estructura del repositorio

```
docs/
├── index.html          ← Viewer (SuperSplat player)
├── index.js            ← Engine de renderizado
├── index.css           ← Estilos
├── scene.compressed.ply ← ⚠️ TU ESCENA (reemplazar)
└── settings.json       ← Posición de cámara inicial
```
