# Guía para subir tu CV a GitHub Pages 🚀

Sigue estos pasos para que tu CV sea accesible desde una URL pública (ejemplo: `https://tu-usuario.github.io/cv_bi/`).

## 1. Requisitos Previos
* Tener una cuenta en [GitHub](https://github.com/).
* Tener instalado [Git](https://git-scm.com/) en tu computadora.

## 2. Crear el Repositorio en GitHub
1. Entra a tu cuenta de GitHub.
2. Haz clic en el botón **"New"** (o el icono `+` arriba a la derecha) para crear un nuevo repositorio.
3. Ponle un nombre, por ejemplo: `cv_bi`.
4. Déjalo como **Public**.
5. **NO** marques las casillas de "Add a README", ".gitignore" o "License" (queremos el repo vacío).
6. Haz clic en **"Create repository"**.

## 3. Subir tus archivos (Consola de comandos)
Abre la terminal (PowerShell o Git Bash) dentro de tu carpeta `C:\Users\DELL\Desktop\cv_bi` y ejecuta estos comandos:

```bash
# 1. Inicializar el repositorio local
git init

# 2. Agregar todos los archivos (index.html y la carpeta certificaciones)
git add .

# 3. Crear el primer commit
git commit -m "Primer subida de CV con certificaciones"

# 4. Crear la rama principal
git branch -M main

# 5. Conectar con tu repositorio de GitHub 
# (Copia la URL de tu repo en GitHub, debe terminar en .git)
git remote add origin https://github.com/TU_USUARIO/cv_bi.git

# 6. Subir los archivos
git push -u origin main
```

## 4. Activar GitHub Pages
Una vez que hayas subido los archivos:
1. En GitHub, ve a la pestaña **Settings** de tu repositorio.
2. En el menú de la izquierda, busca la sección **Code and automation** y haz clic en **Pages**.
3. En la sección **Build and deployment**, asegúrate de que:
   * **Source** diga "Deploy from a branch".
   * **Branch** esté seleccionada la rama `main` y la carpeta `/ (root)`.
4. Haz clic en **Save**.

## 5. ¡Listo! 🌐
Espera unos minutos. GitHub te dará un enlace arriba que dice algo como:
`Your site is live at https://tu-usuario.github.io/cv_bi/`

---
### Notas Importantes:
* **Estructura:** Asegúrate de que el archivo `index.html` esté en la raíz de la carpeta (no dentro de otra subcarpeta).
* **Certificaciones:** Al subir la carpeta `certificaciones`, los enlaces que configuramos en el HTML funcionarán automáticamente en internet.
* **Privacidad:** Recuerda que GitHub Pages es público; cualquier persona con el link podrá ver tu CV y certificados.
