# Visor 3D dental para GitHub Pages

## Archivos
- `index.html`: página con el visor 3D.
- `styles.css`: aspecto visual.
- `modelos/`: carpeta donde debes subir tus archivos `.glb`.

## Preparación
1. Pon un modelo dentro de `modelos/` y llámalo `molar.glb` (o cambia el nombre de archivo en `index.html`).
2. Sube todos los archivos y carpetas a un repositorio de GitHub.
3. En el repositorio, abre **Settings → Pages**.
4. En **Build and deployment**, elige **Deploy from a branch**.
5. Selecciona la rama `main` y la carpeta `/(root)`; guarda.
6. Espera a que GitHub Pages publique la web. La dirección será parecida a `https://TUUSUARIO.github.io/TUREPOSITORIO/`.

## Usar varios modelos
Sube, por ejemplo:
- `modelos/incisivo.glb`
- `modelos/canino.glb`
- `modelos/premolar.glb`
- `modelos/molar.glb`

Luego usa estas URLs:
- `https://TUUSUARIO.github.io/TUREPOSITORIO/?modelo=incisivo.glb`
- `https://TUUSUARIO.github.io/TUREPOSITORIO/?modelo=canino.glb`
- `https://TUUSUARIO.github.io/TUREPOSITORIO/?modelo=premolar.glb`
- `https://TUUSUARIO.github.io/TUREPOSITORIO/?modelo=molar.glb`

Sustituye `TUUSUARIO` y `TUREPOSITORIO` por los tuyos. El nombre de archivo distingue mayúsculas y minúsculas; evita espacios, tildes y ñ en los nombres.

## Insertar en Moodle
En la pregunta, usa el editor HTML y pega algo parecido a esto:

```html
<iframe
  src="https://TUUSUARIO.github.io/TUREPOSITORIO/?modelo=molar.glb"
  title="Modelo dental 3D"
  width="100%"
  height="520"
  style="border:0; max-width:100%;"
  loading="lazy"
  allowfullscreen>
</iframe>
```

Sustituye la URL por la correspondiente. Si Moodle elimina el iframe al guardar, el problema está en los permisos/filtros de Moodle y debe revisarlo el administrador.

## Importante
- Este visor no añade marcas de agua ni etiquetas anatómicas. Si el modelo tiene texto, etiquetas o colores incrustados en la geometría/texturas, seguirán presentes.
- GitHub Pages es público: cualquier persona que conozca la URL puede acceder a la página y a los modelos publicados. No subas material si la licencia no permite redistribuirlo.
- GitHub Pages sirve páginas estáticas; el visor carga `model-viewer` desde Google CDN, por lo que la página necesita conexión a Internet.
- Comprueba la licencia del modelo descargado de Sketchfab antes de volver a publicarlo.
- Para archivos grandes, ten en cuenta los límites de tamaño y uso de GitHub Pages.
