# PEQUE Gestión

Presupuestos, facturas y cuentas de PEQUE Pintura y Decoración. Web publicada en GitHub Pages con los datos en Firebase (igual que la app del club de bádminton).

## Archivos
- `index.html`: la app.
- `firebase-config.js`: datos del proyecto de Firebase (hay que rellenarlo).
- `firestore.rules`: reglas de seguridad para pegar en Firebase.
- `manifest.webmanifest`, `icon-192.png`, `icon-512.png`, `logo.jpg`: icono para instalarla en el móvil y el ordenador.

## 1. Firebase (proyecto nuevo, separado del club)
1. console.firebase.google.com → Agregar proyecto → `peque-gestion`.
2. Compilación → Authentication → Comenzar → Correo electrónico/contraseña → Habilitar.
3. Authentication → Usuarios → Agregar usuario: el email y una contraseña de Oscar. Repite con el tuyo.
4. Copia el "UID de usuario" de cada uno.
5. Compilación → Firestore Database → Crear base de datos → ubicación `europe-southwest1` (Madrid) → modo producción.
6. Firestore → Reglas → pega `firestore.rules`, cambia `UID_DE_OSCAR` y `UID_DE_GERARDO` por los UID → Publicar.
7. Configuración del proyecto → Tus apps → icono `</>` (web) → registrar app → copia los valores de `firebaseConfig` en `firebase-config.js`.
8. Authentication → Configuración → Dominios autorizados → añade `gerardoortega74-rgb.github.io`.

## 2. GitHub Pages
1. Crea el repositorio `peque_gestion` en github.com/gerardoortega74-rgb.
2. Sube todos los archivos de esta carpeta.
3. Settings → Pages → Branch `main` / root → Save.
4. La app queda en `https://gerardoortega74-rgb.github.io/peque_gestion/`.

## 3. Oscar
- Abre el enlace en el móvil y en el ordenador y entra con su email y contraseña.
- Móvil: menú del navegador → "Añadir a pantalla de inicio". Ordenador (Chrome/Edge): icono de instalar en la barra de direcciones.
- Los datos se sincronizan entre móvil y ordenador. Sin internet sigue funcionando y sincroniza al volver la conexión.
