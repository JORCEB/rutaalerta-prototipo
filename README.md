# RutaAlerta · prototipo web

Grupo 7 · Jorge Ceballos, Juan Marinan y Alan Bravo.

Código del prototipo publicado previamente, exportado sin cambiar sus pantallas ni interacciones. HTML, CSS y JavaScript estáticos. No requiere Node, instalación, compilación ni variables de entorno. Utiliza Google Fonts y fuentes de respaldo.

## Publicar en Vercel

Código disponible en https://github.com/JORCEB/rutaalerta-prototipo.

1. Entrar en https://vercel.com/new con la cuenta que conectará este repositorio.
2. Conectar GitHub y autorizar el acceso a `JORCEB/rutaalerta-prototipo`.
3. Importar `rutaalerta-prototipo` con estas opciones:

| Opción | Valor |
| --- | --- |
| Framework Preset | Other |
| Root Directory | Raíz del repositorio (`.`) |
| Build Command | Vacío, sin comando |
| Install Command | Vacío, sin comando |
| Output Directory | public |
| Environment Variables | Ninguna |

4. Pulsar **Deploy** y probar la dirección que entregue Vercel.
5. Comprobar el enlace en una ventana privada. Si exige iniciar sesión, revisar la protección del despliegue de producción para permitir el acceso público deseado.

`vercel.json` incluye la configuración de compilación y salida. Los cambios posteriores enviados a la rama de producción se desplegarán automáticamente si la integración permanece autorizada. La importación inicial debe completarse en Vercel; subir este código a GitHub no publica por sí solo el sitio.

## Archivos

- `public/index.html`: entrada del sitio.
- `public/style.css`: diseño adaptable.
- `public/app.js`: pantallas, datos ficticios y lógica de demostración.
- `vercel.json`: configuración de publicación.

## Probar en el computador

Desde esta carpeta, con Python instalado:

```bash
python -m http.server 8000 --directory public
```

Abrir http://localhost:8000. Detener con Ctrl+C.

## Recorrido de demostración

1. En Ciudadano, registrar un vehículo ficticio y reportar un incidente.
2. En Central, revisar el caso y publicar su solicitud.
3. En Ciudadano, aportar un avistamiento desde Colaborar.
4. En Central, aceptar, rechazar o pedir aclaración con motivo.
5. Consultar avisos y seguimiento desde Ciudadano.
6. Explorar cámaras, recorridos posibles, candidatos, copiloto y métricas en Central.

## Qué representa

Es un prototipo visual interactivo. Usa datos ficticios y estado en memoria que se pierde al recargar. El selector de roles simula las vistas: no es autenticación. El mapa es esquemático; las cámaras, candidatos y respuestas del copiloto son simulaciones. No hay PostgreSQL, FastAPI, GPS real, notificaciones remotas, carga a la nube ni análisis real con IA. Publicarlo en Vercel no incorpora esos servicios. No usar datos personales reales.

La arquitectura del producto final sigue siendo una decisión independiente del alojamiento de esta demostración.

## Verificación de esta exportación

Se comprobó la sintaxis de JavaScript, la configuración JSON y que HTML/CSS/JS son idénticos a la versión publicada de origen. La importación y el despliegue en Vercel no se han ejecutado desde este entorno. No se realizó una nueva prueba visual en navegador.

## Referencias de publicación

- https://vercel.com/docs/builds/configure-a-build
- https://vercel.com/docs/project-configuration/vercel-json
- https://vercel.com/docs/git/vercel-for-github
