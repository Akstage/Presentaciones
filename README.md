# Presentaciones
## Plugin 3 SG - Optimizer

## Pluguin 13 WP Maintenance mode

## Pluguin 34 Widget Importer and Exporter

## Plugin 100
1. Borrar todos los comentarios del sitio de wordpress.
  * Opción 1:
    En todos los sitios; quita los controles y las configuraciones relacionadas con los comentarios.

  * Opción 2:
    En determinados tipos de entradas (entradas, páginas o medios)
    no habrá nada relacionado con los comentarios en la edicion y no puede ponerse para entradas individuales.
2. Recargar la página o al salir del modo admin es cuando se aplican los cambios.

this plugin allows administrators to globally disable comments on any post type (posts, pages, attachments, etc.) so that these settings cannot be overridden for individual posts. It also removes all comment-related fields from edit and quick-edit screens. On multisite installations, it can be used to disable comments on the entire network.

Además, los elementos relacionados con los comentarios pueden ser retirados del escritorio, de los widgets, del menú de administración y de la barra de administrador.

Nota importante: Utilice este plugin si no desea que los comentarios del todo en su sitio (o en ciertos tipos de entradas). No lo use si desea desactivar selectivamente los comentarios sobre los entradas individuales – WordPress te permite hacerlo. Si usted no sabe cómo desactivar los comentarios sobre los entradas individuales, tienes instrucciones en las preguntas frecuentes .

If you come across any bugs or have suggestions, please use the plugin support forum. I can’t fix it if I don’t know it’s broken! Please check the FAQ for common issues.

Want to contribute? Here’s the GitHub development repository.

Una versión imprescindible del plugin también está disponible.
Detalles

The plugin provides the option to completely disable the commenting feature in WordPress. When this option is selected, the following changes are made:

    Todos los enlaces “Comentarios” están ocultos en el menú de administración y la barra de administración;
    Todas las secciones de comentarios relacionados-( “Comentarios recientes”, “Discusión”, etc.) se ocultan en el escritorio de WordPress;
    Todos los widgets relacionados con los comentarios están desactivados (para que tu tema no pueda utilizarlos);
    La página de ajustes de “discusión” está oculta;
    Todos los feeds de RSS/Atom están desactivados (y las solicitudes a éstos serán redirigidos a la entrada padre correspondiente);
    The X-Pingback HTTP header is removed from all pages;
    Outgoing pingbacks are disabled.

Por favor, elimina los comentarios existentes en tu sitio antes de aplicar este ajuste, de lo contrario esos comentarios todavía podrían mostrarse a los visitantes (dependiendo de tu tema). Puedes utilizar la herramienta de eliminación de comentarios para eliminar cualquier comentario existente en tu sitio.
Configuración avanzada

Some of the plugin’s behaviour can be modified by site administrators and plugin/theme developers through code:

    Definir DISABLE_COMMENTS_REMOVE_COMMENTS_TEMPLATE y ponerlo a false para evitar que el plugin sustituya la plantilla de comentarios del tema por una vacía.

    Define DISABLE_COMMENTS_ALLOW_DISCUSSION_SETTINGS and set it to true to prevent the plugin from hiding the Discussion settings page.

These definitions can be made either in your main wp-config.php or in your theme’s functions.php file.
