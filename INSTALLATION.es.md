# Instalación y actualizaciones manuales

EQphile Studio **0.17.8 (40)** — beta para Apple Silicon.

## Descargar y verificar

Descarga ambos archivos de la [publicación oficial de la beta 0.17.8](https://github.com/gmaurotl/EQphileStudio/releases/tag/v0.17.8):

- **EQphileStudio-0.17.8-arm64.zip** — la app compilada para Mac.
- **SHA256SUMS.txt** — el checksum de ese ZIP.

Los archivos **Source code** que genera GitHub contienen la documentación del
repositorio, no la app instalable ni su código fuente privado.

Para verificar el ZIP, abre Terminal en la carpeta que contiene ambos archivos
y ejecuta esta comprobación opcional de integridad:

```sh
shasum -a 256 -c SHA256SUMS.txt
```

Debe aparecer `EQphileStudio-0.17.8-arm64.zip: OK`. Si no coincide, detente y
vuelve a descargar ambos archivos de la misma publicación. El checksum comprueba
la integridad del archivo; no sustituye la firma del desarrollador ni la notarización.

## Instalar la app

1. Abre el ZIP en Finder.
2. Arrastra **EQphile Studio.app** a **Aplicaciones**. El ZIP contiene la app;
   no hay instalador, clave de activación ni paso de pago.
3. Abre EQphile Studio desde Aplicaciones.

Esta beta tiene **firma ad hoc, sin Developer ID ni notarización de Apple**.
macOS puede bloquear su primera apertura. La [guía de Apple](https://support.apple.com/es-es/102445)
explica la excepción para una app concreta en Ajustes del Sistema → Privacidad
y seguridad, si decides confiar en ella. No desactives Gatekeeper globalmente.
Si macOS indica que dañará el ordenador, detente e informa del aviso exacto a soporte.
La primera apertura en otro Mac o con un usuario nuevo no se ha verificado.

## Primer uso

- **Archivos locales:** añade un archivo de audio desde Biblioteca o Reproductor.
- **Spotify:** abre su app de escritorio, reproduce una pista y selecciona Spotify en Studio.
- **Música / Apple Music:** reproduce una pista en Música y selecciona esa fuente en Studio.
- **Navegador / YouTube:** reproduce contenido en un navegador compatible y selecciona esa fuente.
- **Audio del Mac:** actívalo por separado para procesar el sonido de otras apps.
  Concede el permiso de audio del sistema cuando macOS lo solicite para esta función.

Los controles de Spotify y Música requieren sus respectivos permisos de
Automatización de macOS. El acceso al streaming corresponde a esas apps; Studio
no proporciona suscripciones. Consulta los límites, la disponibilidad de
carátulas y las versiones de macOS probadas en [Compatibilidad](COMPATIBILITY.es.md).

## Actualizar manualmente

Las consultas públicas de actualización están desactivadas en esta compilación;
no descarga ni instala actualizaciones automáticamente. Para usar otra versión:

1. Descarga el ZIP y el archivo de checksum correspondiente a esa publicación.
2. Verifica la descarga y sal de Studio con **⌘Q** antes de reemplazarla.
3. Sustituye la app instalada en Aplicaciones y abre la versión nueva.

Reemplazar la app no requiere borrar tu música original, preferencias o
preajustes. Lee las notas de cada versión por si incluye pasos de migración.

## Soporte y condiciones

Todas las funciones incluidas son gratuitas y el código de la aplicación sigue
siendo privado. Consulta las [condiciones del binario](LICENSE.txt), la
[privacidad](PRIVACY.md) y los [avisos de terceros](NOTICE.md), también disponibles
sin conexión en el menú Ayuda de la app. Los textos legales completos están en inglés.

Soporte: **eqphile@maurotarazona.com**.

Web del desarrollador: [maurotarazona.com](https://maurotarazona.com).
