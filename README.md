# CV estático — Facundo Diorio

Este repositorio contiene una versión simple y desplegable del CV de Facundo Diorio. Está pensada para deploy inmediato en servicios gratuitos como Vercel o GitHub Pages.

Contenido
- `index.html` — Página estática del CV
- `styles.css` — Estilos básicos
- `data.txt` — Versión texto del CV (editable)

Despliegue rápido (opciones)

1) Vercel (recomendado)
- Conecta tu cuenta de GitHub y haz import del repositorio. Vercel detecta que es un sitio estático y lo despliega automáticamente.

2) GitHub Pages
- Pasos (PowerShell):

```powershell
git init
git add .
git commit -m "Add static CV"
git branch -M main
# Crea un repo en GitHub y luego añade el remote (reemplaza URL)
git remote add origin https://github.com/FacuDee/nombre-repo-cv.git
git push -u origin main
```

Luego en GitHub > Settings > Pages, seleccioná la rama `main` y la carpeta `/ (root)` como fuente. GitHub Pages tardará unos minutos en publicar.

3) Netlify
- Arrastrá la carpeta al panel de Netlify Drop o conecta el repo de GitHub para deploy automático.

Notas
- Si querés que genere un PDF listo para descargar desde `index.html` puedo crearlo y añadirlo al repo.
- También puedo preparar un `package.json` mínimo y script de build si querés usar Vite u otro bundler.
