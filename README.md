# Sitio personal de Alejandra González Jiménez

Sitio estático con Jekyll y el tema Moon.

## Comentarios

Los comentarios están desactivados por ahora. `disqus_shortname` está vacío
en `_config.yml` y la entrada actual usa `comments: false`. El sitio generado
no carga Disqus ni muestra el recuadro o el aviso de comentarios.
La página de contacto sigue disponible para escribir por correo.

## Google Analytics 4

El identificador configurado es `G-35KSFJTJEK`. La etiqueta se incluye una sola
vez en la cabecera de cada página mediante `_includes/analytics.html`.

1. En Google Analytics, selecciona la propiedad de este sitio.
2. En Administrar → Flujos de datos → Web, confirma que el ID de medición
   coincide con `G-35KSFJTJEK` y que la dirección es `https://alejandragj.com`.
3. Después de publicar, abre el sitio en otro navegador sin bloqueadores y
   revisa el informe En tiempo real. Si no ves visitas, usa Google Tag Assistant
   o DebugView siguiendo la guía de Google.
4. Consulta visitas por página, adquisición y participación en los informes
   de Analytics. Los datos se consultan en tu cuenta; no hay un panel público
   de métricas en el sitio.

La instalación del código no verifica el acceso a la propiedad ni recupera
visitas pasadas que no se hayan registrado.

Guía oficial: https://developers.google.com/analytics/devguides/collection/ga4/troubleshoot

## Contacto

La página `/contacto/` y el menú usan `email` de `_config.yml`, actualmente
`heliconideu@gmail.com`. El botón abre la aplicación de correo del visitante;
no almacena ni envía mensajes desde un servidor. También muestra el Instagram
configurado en el sitio.

## Página de actividad

El contenido está en `_posts/2016-03-21-moon-theme.md`. Conserva `/moon-theme/`
para mantener sus enlaces. El campo `updated` controla la fecha visible;
`date` conserva la fecha original del archivo. Los estilos específicos están
en `_sass/personal.scss`.

## Generación y publicación

El Gemfile conserva Jekyll 3.6.3. Necesita un entorno de Ruby compatible con
sus dependencias antiguas; Ruby 4 requiere adaptaciones para ejecutarlo.
Con el entorno compatible instalado: `bundle install` y `bundle exec jekyll build`.

Los cambios locales no actualizan automáticamente el dominio. Publica a través
del repositorio y la rama configurados en GitHub Pages, y comprueba el resultado
del despliegue antes de verificar Analytics y Disqus en el dominio.
