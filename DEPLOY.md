# Cómo desplegar Himalaya Rutero en Vercel

Para compartir tu aplicación con amigos, la forma más fácil y gratuita es usar **Vercel**.

## Opción 1: Despliegue desde GitHub (Recomendado)

1.  **Crea un repositorio en GitHub**:
    *   Ve a [github.com/new](https://github.com/new).
    *   Ponle un nombre (ej: `himalaya-rutero`).
    *   No marques "Initialize with README" ni ".gitignore" (ya los tenemos).
    *   Dale a "Create repository".

2.  **Sube tu código**:
    Abre una terminal en esta carpeta y ejecuta:
    ```bash
    git remote add origin https://github.com/TU_USUARIO/himalaya-rutero.git
    git branch -M main
    git push -u origin main
    ```
    *(Reemplaza TU_USUARIO con tu nombre de usuario de GitHub)*

3.  **Conecta con Vercel**:
    *   Ve a [vercel.com/new](https://vercel.com/new).
    *   Selecciona tu repositorio `himalaya-rutero`.
    *   Dale a **Import**.
    *   En "Environment Variables" (Variables de Entorno), añade:
        *   `NEXT_PUBLIC_PARTICIPANT_ID` = `Participant-001` (o lo que quieras).
    *   Haz clic en **Deploy**.

## Opción 2: Despliegue desde Terminal (Vercel CLI)

Si tienes instalado Node.js, puedes hacerlo directamente:

1.  Instala Vercel CLI:
    ```bash
    npm i -g vercel
    ```
2.  Ejecuta el comando de despliegue:
    ```bash
    vercel
    ```
3.  Sigue las instrucciones en pantalla (Login, Link to existing project? [No], etc.).

¡Y listo! Vercel te dará una URL (ej: `himalaya-rutero.vercel.app`) que podrás enviar por WhatsApp a tus amigos.
