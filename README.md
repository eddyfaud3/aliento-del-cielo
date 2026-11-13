# Aliento del Cielo

Proyecto independiente para preparar historias bíblicas en español y convertirlas, en una siguiente etapa, en videos verticales para Facebook.

## Estado inicial

- Repositorio separado de `mundo-al-dia`.
- Flujo inicial manual: no publica en Facebook ni Instagram.
- Los guiones deben respetar el pasaje bíblico y distinguir el texto bíblico de la reflexión.
- Formato editorial previsto: Reels verticales 9:16, narración masculina natural en español y duración objetivo de 1–2 minutos.
- La generación de voz/video con IA y la publicación automática se integrarán después de configurar proveedores, credenciales y permisos.

## Primer flujo

En GitHub Actions, ejecuta **Crear borrador de historia bíblica** y completa los campos. El flujo empaqueta el borrador como un archivo descargable. No publica nada.

## Próximas etapas

1. Conectar un proveedor de IA para investigar y redactar guiones con referencias verificables.
2. Conectar generación de voz en español.
3. Crear escenas visuales y montar un MP4 vertical compatible con iPhone.
4. Revisar calidad, fidelidad bíblica y derechos de medios.
5. Añadir publicación a la página de Facebook solo después de pruebas y autorización explícita.

## Seguridad

Nunca guardes tokens, contraseñas, claves de API ni credenciales de Meta en archivos del repositorio. Usa GitHub Actions Secrets cuando llegue el momento.
