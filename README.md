# Nexus Card System — Versión 5

Este sistema permite la gestión segura y controlada de solicitudes para una tarjeta virtual personalizada ("Nexus Card"). Está diseñado para permitir acceso solo a usuarios autorizados, limitar duplicados y ofrecer control completo al administrador.

---

## ✨ Funcionalidades principales

### 👤 Acceso de usuario (login)
- Acceso restringido por ID autorizado (definido en el código)
- Un solo intento de solicitud por ID
- Mensajes inteligentes según el estado:
  - ❌ No autorizado
  - ⏳ Solicitud pendiente
  - ✅ Solicitud aprobada
  - 🚫 Eliminado: no puede reenviar

### 📝 Formulario de solicitud
- Campos: ID (rellenable), Apodo, Usuario, País, Fecha de nacimiento, Imagen
- Validación de todos los campos
- Imagen se comprime automáticamente antes de enviarse
- Confirmación al enviar: `"✅ Solicitud enviada para aprobación"`

### 📥 Envío a Firestore (Firebase)
- Todos los datos se guardan con el ID del usuario como clave
- Evita duplicados automáticamente

---

## 🛠 Panel de administración (requiere clave: `Prefijo_123`)
- Ver todas las solicitudes
- Botones para:
  - ✅ Aprobar
  - 🗑️ Eliminar
  - 📥 Descargar imagen enviada
- Las solicitudes persisten al recargar
- Cambios reflejados en la experiencia del usuario automáticamente

---

## 🎨 Interfaz visual
- Títulos personalizados con logo
  - `"Login"` (en la entrada)
  - `"Solicitar Nexus Card"` (en el formulario)
- Logo visible a la izquierda de cada título
- Campos y botones correctamente alineados y centrados
- Botones con efectos visuales (hover, pointer, active)

---

## 🚀 Hosting y despliegue
- El sistema está listo para subirse a GitHub
- Se puede desplegar fácilmente en Netlify
- Compatible con Firebase Firestore (web SDK)

