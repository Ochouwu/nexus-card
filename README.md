# Nexus Card System

Sistema web para gestionar solicitudes con acceso restringido por ID.

## Funcionalidad

- ✅ Solo los IDs autorizados pueden enviar solicitud
- ✅ Solo una solicitud por ID
- ✅ Panel de administración con clave: `Prefijo_123`
- ✅ Puedes aprobar o eliminar solicitudes
- ✅ Se guarda todo en Firebase (Firestore)
- ✅ Listo para desplegar en Netlify

## Archivos

- `index.html` — Página principal (formulario + panel admin)
- `README.md` — Este archivo

## Uso

1. Edita la lista `autorizados = [...]` en `index.html` con los IDs permitidos.
2. Usa la clave `Prefijo_123` para entrar al modo administrador.
3. Sube este proyecto a GitHub y luego conéctalo a Netlify para publicar la web.

## Despliegue en Netlify

1. Crea un nuevo sitio en [Netlify](https://app.netlify.com/).
2. Importa tu repositorio de GitHub.
3. No necesitas comandos de build, solo asegúrate que `index.html` está en la raíz.
4. ¡Publica tu sitio y comienza a usarlo!
