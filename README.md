# Jarvis Echo

Asistente de voz con Claude para el **Echo Show 5 con LineageOS** (y otras tablets Android 8 o superior).
Todo en **una sola app**: oye «Jarvis», habla con Claude usando **tu suscripción de claude.ai** y maneja el
dispositivo (apps, música, volumen, brillo, luz, alarmas, temporizadores y cualquier app en pantalla).

## Descargar

**[⬇ JarvisEcho.apk](https://github.com/carbollo/jarvis-echo/releases/latest/download/JarvisEcho.apk)**

En el Echo Show, escribe esta dirección en el navegador:

```
github.com/carbollo/jarvis-echo/releases/latest/download/JarvisEcho.apk
```

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
   3. **Claude:** pulsa **Abrir Claude** e inicia sesión **con tu correo** (los botones de Google y Apple no
      funcionan dentro de apps). Abre el enlace del correo en el móvil: te mostrará un código; escríbelo en
      el Echo Show.
4. En Claude (desde el Echo, el móvil o el PC): **Ajustes → Conectores → Añadir conector personalizado**,
   nombre `Echo Show` y la URL de tu conector. Después pon **Permitir siempre** en sus herramientas.

## Uso

Di **«Jarvis»** y lo que quieras, de un tirón o con una pausa (suena un pitido cuando te escucha):

- «Jarvis, pon un temporizador de diez minutos.»
- «Jarvis, pon música relajante.»
- «Jarvis, baja el volumen al veinte por ciento.»
- «Jarvis, ¿qué tengo mañana en el calendario?»
- «Jarvis, abre YouTube y busca recetas de lentejas.»

También puedes pulsar **Hablar** en la app o pulsar dos veces **Volumen +**. «Jarvis, para» corta la
respuesta; «Jarvis, repite» la repite; «Jarvis, nueva conversación» empieza un chat nuevo.

## Privacidad

- El reconocimiento de voz y la voz de Jarvis funcionan dentro de la app: el audio no sale del dispositivo.
  A Claude solo llega el texto de lo que dices.
- La sesión de claude.ai la guarda el componente web de Android, como en cualquier navegador. Jarvis no la
  lee ni la envía a ningún sitio.
- Este instalador no lleva dentro ninguna dirección ni clave: el relay y el código de acceso se escriben en
  el propio dispositivo.

## Componentes incluidos

Modelo de voz Vosk, sintetizador Pico de AOSP y otras librerías libres: ver
[THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md).
