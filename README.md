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

## Generación de voz en español

Se eligió **ElevenLabs Multilingual v2** para narraciones largas y expresivas. La voz recomendada para iniciar es **Alberto Rodríguez**: masculina, seria y narrativa, descrita por ElevenLabs como latinoamericana. La voz exacta debe probarse con un fragmento bíblico antes de adoptarla definitivamente.

El flujo **Generar narración bíblica en español** crea un MP3 y lo guarda como artefacto descargable; no publica nada. Utiliza el modelo `eleven_multilingual_v2`, idioma `es` y ajustes moderados para mantener una lectura clara, cálida y natural.

Antes de ejecutarlo, añade estos dos secretos en **Settings → Secrets and variables → Actions** del repositorio:

- `ELEVENLABS_API_KEY`: tu clave API de ElevenLabs.
- `ELEVENLABS_VOICE_ID`: el ID de la voz Alberto Rodríguez copiado desde ElevenLabs.

No pegues las claves en los archivos ni en el chat. El ID de voz no se ha supuesto ni inventado: debes copiar el ID exacto que muestra tu cuenta para esa voz.

## Próximas etapas

1. Probar el MP3 con una narración bíblica corta y comprobar pronunciación, acento y emoción.
2. Conectar investigación y redacción de guiones con referencias verificables.
3. Crear escenas visuales y montar un MP4 vertical compatible con iPhone.
4. Revisar calidad, fidelidad bíblica y derechos de medios.
5. Añadir publicación a la página de Facebook solo después de pruebas y autorización explícita.

## Seguridad

Nunca guardes tokens, contraseñas, claves de API ni credenciales de Meta en archivos del repositorio. Usa GitHub Actions Secrets.
