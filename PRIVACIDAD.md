# Privacidad: skill «Encendido de la PC»

La skill solo sirve para encender por voz una PC con Wake-on-LAN desde tu Echo.

**Qué guarda** (en una tabla de Amazon Web Services, región us-east-1; si tu Alexa es de Europa, la orden pasa por la región eu-west-1, que lee esa misma tabla):

- El identificador de tu cuenta de Amazon que da Login with Amazon (`user_id`). No guarda tu nombre ni tu correo.
- De cada PC que vinculas desde su panel: un identificador aleatorio, el nombre que le pongas y las direcciones MAC de sus tarjetas de red.
- Los permisos que Alexa concede a la skill para enviar el aviso de encendido (tokens de Amazon).
- Si vinculas la PC desde su panel (versión 1.5 o más nueva), para el **panel en internet**: el resumen de un código de la PC (no el código), la hora de su último aviso y su estado mientras está encendida (uso y temperatura del procesador y la gráfica, memoria y disco en porcentaje, tiempo encendida y si hay una cuenta atrás), además de la última orden que dejaste (apagar o cancelar) hasta que la PC la recoge. Cada estado nuevo reemplaza al anterior: no se guarda historial.
- Al entrar al panel en internet, una cookie de sesión firmada con tu identificador de Amazon (30 días).

**Para qué:** decirle a Alexa qué equipos puede despertar y enviar la señal de encendido cuando lo pides. No se comparte con nadie ni se usa para otra cosa.

**Borrarlo:** desactiva la skill en la app Alexa, o pide el borrado abriendo una incidencia en [este repositorio](https://github.com/Daniiel18/alexa-apagar-pc/issues).

El resto del proyecto (el agente de la PC) no envía datos fuera de tu red: habla directamente con tu Echo.

Ver también los [términos de uso](TERMINOS.md).
