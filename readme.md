SportivaX · Chatbot de FAQs (Botpress + Replit)

Demo pública de un chatbot de Preguntas Frecuentes para una tienda deportiva ficticia, SportivaX.
El bot se ha creado en Botpress Cloud y se incrusta en una página web alojada en Replit.

✨ ¿Qué incluye?

5 FAQs principales: horarios, precios, contacto, devoluciones y ubicación.

Conocimiento extendido (productos, envíos, tallas, tarjetas regalo, etc.) cargado en Knowledge Base.

Widget Webchat de Botpress (v3.2) incrustado en una landing moderna.

Instrucciones para replicar y probar.

🔗 Demo

En Replit, pulsa Run.

En el panel de vista previa, pulsa Open in new tab ↗️.

Comparte la URL pública que se abre [(https://99e6031c-d0ab-4ba5-9aba-09b29879dddf-00-1594ocndteg7u.spock.replit.dev/)]

✅ Requisitos

Cuenta en Botpress Cloud (plan gratuito).

Cuenta en Replit (plan gratuito).

📁 Estructura
/ (raíz)
├─ index.html       # Landing con el widget incrustado
└─ README.md        # Este archivo

1) Configurar el bot en Botpress

Crea un bot nuevo (plantilla vacía, idioma español).

Ve a Knowledge Bases → New Knowledge Base → Add Knowledge Source → Rich Text.

Pega el contenido de FAQs y conocimiento (horarios, tiendas en Málaga, devoluciones, productos, etc.).

Abre Emulator y prueba:

“¿Cuál es su horario?”

“¿Dónde están las tiendas en Málaga?”

“Precios de zapatillas”

Pulsa Publish.

En el panel del bot → Webchat → pestaña Share → copia el snippet (v3.2).

Nota: En v3.2 el snippet son dos <script>: uno a inject.js y otro a un .js con tu configuración. No necesitas window.botpressWebChat.init.

2) Publicar la demo en Replit

En Replit → Create App → plantilla HTML, CSS, JS.

Abre index.html, borra su contenido y pega el HTML de la landing (el que estás usando).

En el bloque marcado como “Pega aquí tu snippet real de Botpress (v3.2)”, pega exactamente tus dos líneas <script> de Botpress.

Pulsa Run y abre la URL pública con Open in new tab.

3) Cómo probar (sugerencias de prompts)

“¿Cuál es su horario?”

“¿Dónde están en Málaga?”

“Precios de zapatillas”

“Política de devoluciones”

“Contacto del soporte”

“¿Hacen envíos a domicilio?”

“Guía de tallas”

🎨 Personalización

Edita textos/horarios/direcciones directamente en la Knowledge Base.

En Webchat → Theme puedes cambiar colores, avatar y nombre del bot.

La landing (index.html) usa estilos embebidos; ajusta fuentes, colores o logos a tu marca.

🧰 Solución de problemas

No aparece el botón del chat
Asegúrate de haber pegado ambos <script> del snippet v3.2 en index.html, sin cortar líneas.

El bot no reconoce una pregunta
Añade esa formulación en Knowledge Base (o en Q&A si lo usas) y Publish de nuevo.

Los cambios no se ven
Repite Publish en Botpress y luego refresca la página en Replit.

Error de CORS / carga
Verifica que el primer <script> apunta a: 
https://cdn.botpress.cloud/webchat/v3.2/inject.js
y el segundo a un dominio https://files.bpcontent.cloud/... (tu archivo de configuración).

Render móvil
La landing es responsive. Si el widget tapa contenido, ajusta márgenes inferiores en CSS.

🔒 Licencia

Uso educativo / demo.
