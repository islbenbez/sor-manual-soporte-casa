# b0-0.1 · Metodología y estructura

- **Alumno:* islam benbeztout
- **Bloque:** B0 — Prerrequisitos
- **Fase / ejercicio:****Fase / ejercicio:** Fase 0.8 · B0.P01 Casa (Préstamo de portátiles con Git)
- **Fecha de inicio:** 26/10/2026
- **Fecha de entrega:** 26/10/2026

---

## 🎯 Qué se pedía

Crear desde cero la bóveda `Boveda_HTML_Casa` con su propio repositorio Git en `01_Proyecto`, conectar un repositorio remoto en GitHub (`sor-web-prestamo-portatiles-casa`) por SSH y registrar tres versiones evolutivas de una web interna de préstamo de portátiles. Además, verificar las exclusiones de archivos multimedia con `.gitignore`, inspeccionar el historial navegando entre commits y grabar un vídeo explicativo del proceso.

## ⌨️ Comandos y pasos importantes

- `git --version`, `git config`, `ssh -T git@github.com` — Comprueban la versión de Git, la identidad global del autor y la autenticación SSH con GitHub.
- `pwd` — Muestra la ruta actual para confirmar que se está trabajando dentro de `Boveda_HTML_Casa/01_Proyecto`.
- `git init` — Inicializa el repositorio local en la carpeta `01_Proyecto`.
- `git branch -M main` — Renombra y establece la rama principal como `main`.
- `git status` — Muestra el estado del árbol de trabajo y del área de preparación (_staging area_).
- `git remote add origin git@github.com:USUARIO/sor-web-prestamo-portatiles-casa.git` — Vincula el repositorio local con el remoto SSH en GitHub.
- `git remote -v` — Comprueba las URLs de lectura y envío del remoto `origin`.
- `git add.

## 🛠️ Qué he hecho

(Los pasos que has seguido. No copies el enunciado: cuenta lo que hiciste tú.)

## 🚩 Qué me ha fallado y cómo lo he resuelto

- **Comprobación inicial:** Inicié la grabación en OBS y ejecuté en Git Bash los comandos `git --version`, `git config` y `ssh -T git@github.com` para verificar entorno, identidad y clave SSH.
- **Estructura e inicialización:** Creé en Obsidian la bóveda `Boveda_HTML_Casa` con las carpetas `00_Grabaciones` (fuera de Git), `01_Proyecto`, `01_Proyecto/00_Bitacora` y `01_Proyecto/web`.
- **Ficheros iniciales:** Configuré `.gitignore` para excluir vídeos (`*.mp4`) y creé la primera versión de `web/index.html` ("Equipo 01: disponible.").
- **Primera entrega (Versión 1):** Accedí a `01_Proyecto`, verifiqué la ruta con `pwd`, ejecuté `git init`, renombré a `main`, vinculé el remoto `origin` y realicé el primer `git commit` y `git push`.
- **Segunda entrega (Versión 2):** Cambié el estado en `index.html` a "reservado para mantenimiento", verifiqué con `git diff`, y subí la segunda entrega con `git add`, `git commit` y `git push`.
- **Ampliación y prueba de exclusiones (Versión 3):** Creé `normas.html`, `contacto.html`, añadí `portatil.png` en `imagenes/` y dos archivos `.mp4` en `videos/`. Comprobé con `git check-ignore` que los vídeos quedaban excluidos.
- **Confirmación de la ampliación:** Preparé los 4 archivos individualmente con `git add`, revisé la selección con `git diff --cached --stat` y subí el tercer commit a GitHub.
- **Navegación por el historial:** Consulté el historial con `git log --oneline`, viajé al primer commit con `git switch --detach` para comprobar el estado inicial en el navegador y regresé a la actualidad con `git switch main`.
- **Cierre:** Detuve la grabación, subí el vídeo a YouTube como "No listado", completé la descripción con las marcas de tiempo y guardé el commit final con la bitácora terminada.

## **🚩 Qué me ha fallado y cóm**

## 🤔 Respuestas a las preguntas

1- **¿Por qué** **git init** **se hizo en** **01_Proyecto** **y no en la raíz de la bóveda?** Se ejecutó en `01_Proyecto` porque es la carpeta destinada al código web y su documentación cuyo historial debe controlarse. La raíz de la bóveda (`Boveda_HTML_Casa`) contiene la configuración interna de Obsidian (`.obsidian/`) y las grabaciones (`00_Grabaciones/`), las cuales deben quedar fuera de Git.
- **¿Qué mostró** **git status** **antes de** **add** **, después de** **add** **y después de** **commit** **?**
- **Antes de** **add** **:** Mostró los archivos sin seguimiento (_untracked_) `??` o modificados no preparados `[ ]M`.
- **Después de** **add** **:** Mostró los archivos en el área de preparación (_staged_), marcados como `A[ ]` (nuevos) o `M[ ]` (modificados).
- **Después de** **commit** **:** Mostró un estado limpio (_working tree clean_), indicando que no quedaban cambios pendientes.
- **¿Por qué creaste un repositorio de GitHub propio y lo conectaste con** **git remote add origin** **?** Porque se requería un repositorio remoto en GitHub (`sor-web-prestamo-portatiles-casa`) para publicar y respaldar el proyecto de casa. El comando `git remote add origin` vincula la dirección SSH local con ese repositorio específico de GitHub para permitir los envíos con `git push`.
- **¿Por qué las páginas nuevas aparecen en** **git status** **pero no en** **git diff -- web/index.html** **?** `git status` informa sobre el estado global de todos los archivos del repositorio. Por su parte, `git diff -- web/index.html` compara únicamente las modificaciones en el archivo `index.html` frente a su versión en el índice o commit, omitiendo otros archivos nuevos sin seguimiento.
- **¿Cómo has comprobado que los vídeos existen pero no se van a subir?** Mediante el comando `git check-ignore -v web/videos/revision-01.mp4 web/videos/revision-02.mp4`. Este comando confirma qué regla de `.gitignore` (`*.mp4`) y en qué línea se aplica para excluir ambos vídeos. Se verificó también en el explorador de archivos que los vídeos siguen almacenados localmente.
- **¿Qué muestra** **git diff --cached --stat** **después de preparar los cuatro archivos?** Muestra un resumen estadístico de los cambios preparados en el índice (_staged_), listando los cuatro archivos (`index.html`, `normas.html`, `contacto.html` y `portatil.png`) y las líneas añadidas o modificadas en cada uno.
- **¿Qué cambia al visitar el primer commit y qué recuperas al volver a** **main** **?**
- **Al visitar el primer commit (** **git switch --detach
2.
3.

## 🔗 Enlaces

- **Vídeo de esta fase:** https://youtu.be/XXXXXXXXXXX
- **Playlist:** B0_Prerrequisitos

## 💭 Dudas / a repasar

- (lo que no te ha quedado claro)