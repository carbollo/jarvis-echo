# Jarvis Echo

Asistente de voz con Claude para el **Echo Show 5 con LineageOS** (y otras tablets Android 8 o superior).
Todo en **una sola app**: oye «Jarvis», habla con Claude usando **tu suscripción de Claude** y maneja el
dispositivo (apps, música, volumen, brillo, luz, alarmas, temporizadores y cualquier app en pantalla).

## Descargar

**[⬇ JarvisEcho.apk](https://github.com/carbollo/jarvis-echo/releases/latest/download/JarvisEcho.apk)**

En el Echo Show, escribe esta dirección en el navegador:

```
github.com/carbollo/jarvis-echo/releases/latest/download/JarvisEcho.apk
```

Para actualizar, descarga la versión nueva desde la misma dirección e instálala encima: se conservan los
ajustes y la conexión.

## Instalar en el Echo Show

1. Abre la dirección de arriba en el navegador del Echo Show y descarga `JarvisEcho.apk`.
2. Abre el archivo descargado. Si Android avisa de que el navegador no puede instalar apps, pulsa
   **Ajustes**, activa **Permitir de esta fuente**, vuelve atrás y pulsa **Instalar**.
3. Abre **Jarvis Echo** y sigue la tarjeta **Para empezar**:
   1. **Permisos:** pulsa **Activar** en cada permiso de la lista hasta que todos tengan ✓
      (accesibilidad, micrófono, brillo, batería y mostrar sobre otras apps). En el micrófono elige
      «Mientras se usa la app».
   2. **Relay:** escribe la **dirección del relay** y el **código de acceso** (te los da quien montó tu
      relay) y pulsa **Guardar y conectar**. Arriba debe poner **Conectado**.
4. **Modo claude.ai (opcional).** Si tu relay tiene Claude Code en un servidor, Jarvis contesta con él y
   esto no hace falta. Sirve para usar claude.ai dentro de la app y tus conectores de claude.ai (Gmail,
   Calendar…), que solo funcionan en este modo:
   1. Pulsa **Abrir Claude** e inicia sesión **con tu correo** (los botones de Google y Apple no
      funcionan dentro de apps). Abre el enlace del correo en el móvil: te mostrará un código; escríbelo en
      el Echo Show.
   2. En Claude (desde el Echo, el móvil o el PC): **Ajustes → Conectores → Añadir conector
      personalizado**, nombre `Echo Show` y la URL de tu conector. Después pon **Permitir siempre** en sus
      herramientas.
   3. En Jarvis Echo, desactiva **Usar Claude Code del servidor**.

## Uso

Di **«Jarvis»** y lo que quieras, de un tirón o con una pausa (suena un pitido cuando te escucha):

- «Jarvis, pon un temporizador de diez minutos.»
- «Jarvis, pon música relajante.»
- «Jarvis, baja el volumen al veinte por ciento.»
- «Jarvis, ¿qué noticias hay hoy?»
- «Jarvis, abre YouTube y busca recetas de lentejas.»

Jarvis empieza a hablar en cuanto llega la primera frase de la respuesta. Después te escucha unos segundos
sin que repitas «Jarvis», para seguir la conversación; di **«gracias»** para terminar.

También puedes pulsar **Hablar** en la app o pulsar dos veces **Volumen +**. «Jarvis, para» corta la
respuesta; «Jarvis, repite» la repite; «Jarvis, nueva conversación» empieza una conversación nueva.

Si tu relay tiene una clave de Groq, Jarvis transcribe cada orden con **Whisper**, que entiende muchísimo
mejor que el reconocedor del Echo (interruptor **Entender mejor con Whisper**). Sin conexión, usa el del
Echo.

Si le cuesta oír «Jarvis», sube su sensibilidad en la app; si se activa solo, bájala. **Reducir ruido del
micrófono** ayuda si hablas de lejos o hay ruido de fondo.

## Privacidad

- «Jarvis» se detecta dentro de la app, y la voz de Jarvis también suena desde la app. Con Whisper
  activado, el audio de cada orden (solo lo que dices después de «Jarvis») va a Groq para transcribirlo.
  Sin Whisper, el audio no sale del dispositivo. A Claude solo llega el texto de lo que dices.
- Jarvis no guarda ni ve tu cuenta de Claude. En el modo claude.ai, la sesión la guarda el componente web
  de Android, como en cualquier navegador, y Jarvis no la lee ni la envía a ningún sitio.
- Este instalador no lleva dentro ninguna dirección ni clave: el relay y el código de acceso se escriben en
  el propio dispositivo.

## Componentes incluidos

Modelo de voz Vosk, sintetizador Pico de AOSP y otras librerías libres: ver
[THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md).
