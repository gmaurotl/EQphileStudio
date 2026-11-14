# Compatibilidad y alcance de la beta

**EQphile Studio 0.17.8 beta (40)**.
EQphile Studio está diseñada para Mac con Apple Silicon. Esta compilación no
admite Intel. El requisito técnico de compilación es macOS 14.2; eso no demuestra
que se haya probado cada versión posterior.

| Entorno | Estado |
| --- | --- |
| macOS 27.0.1 y Apple Silicon, Mac de desarrollo | Se han probado la interfaz nativa e integraciones de fuentes en este Mac. La 0.17.8 pasó las comprobaciones de versión y las pruebas simuladas de Spotify y del navegador. No se ha probado la primera apertura desde una descarga en otro Mac. |
| Otras versiones de macOS desde 14.2 | Sin verificar; no prometemos compatibilidad. |
| macOS anterior a 14.2 | No compatible. |
| Mac con Intel | No compatible. |

## Fuentes y permisos

- **Archivos locales:** mono/estéreo; hasta 256 MiB de PCM float32 decodificado.
- **Spotify:** app de escritorio y permiso de Automatización de macOS. Las
  carátulas usan los servidores de imágenes de Spotify admitidos; los controles
  disponibles dependen de la fuente y del servicio.
- **Música / Apple Music:** app Música del Mac y permiso de Automatización.
  Incluye metadatos, carátula disponible, pausa/reanudación, anterior/siguiente,
  desplazamiento por la pista, aleatorio y repetición desactivada/de todas/de una.
  Música proporciona el contenido de suscripción bajo sus condiciones. La
  carátula procede solo de Música o de información local coincidente de macOS;
  algunas pistas pueden no tener una imagen disponible.
- **Navegador / YouTube:** depende de Ahora suena de macOS, del navegador, de la
  fuente y de los controles que publique. No necesita extensiones. La integración
  usa un adaptador incluido para API privadas del sistema; los cambios de macOS
  pueden afectar a su funcionamiento.
- **Audio del Mac:** permiso de audio del sistema; se activa por separado de la
  selección de fuente. Los formatos de salida dependen del dispositivo de audio.

## Alcance de las pruebas

La primera apertura en otro Mac o con un usuario nuevo no se ha verificado.
Tampoco se han verificado otras versiones de macOS ni otros equipos de audio
con esta beta.

Para informar de un fallo, incluye versiones de la app y macOS, chip del Mac,
fuente, dispositivo de salida y pasos. Envía los detalles privados a
**eqphile@maurotarazona.com**; consulta [Soporte](SUPPORT.md).

## Disponibilidad de controles de Spotify

La 0.17.8 comprueba fuente, proceso, pista y acciones disponibles. No identifica
ni certifica una suscripción Premium. Las capacidades ausentes, caducadas o
restringidas mantienen deshabilitado el control afectado. Si macOS o Spotify
no publican información coincidente, usa Abrir Spotify. La posición se sigue
mostrando. Las pruebas usan contextos simulados; no se repitieron pruebas de
cuenta real de Spotify, salida de audio o escucha.
