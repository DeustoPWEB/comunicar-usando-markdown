## Paso 3: Añade encabezados

Como has podido ver en tu sitio web, tu portafolio no tiene mucho contenido todavía. Aprenderemos a editar un archivo en esta solicitud de extracción para incorporar algunos encabezados en Markdown.

Puedes ver un ejemplo de encabezado en la parte superior de esta página. Exactamente igual que en HTML, un encabezado es un fragmento de texto un poco más grande al principio de una sección. Hay seis tamaños.

#### Ejemplo

```
# Esto es un encabezado <h1>, que es el más grande
## Esto es un encabezado <h2>
###### Esto es un encabezado <h6>, que es el más pequeño
```

#### Cómo se muestra

# Esto es un encabezado <h1>, que es el más grande
## Esto es un encabezado <h2>
###### Esto es un encabezado <h6>, que es el más pequeño

En propuestas (o _issues_), solicitudes de extracción (o _pull requests_) y comentarios puedes usar la barra de herramientas de formato.

La barra de herramientas no está disponible en todas partes. Cuando editas un archivo, tienes que teclear los caracteres `#` manualmente.

### :keyboard: Actividad: Edita tu archivo con encabezados

{% if preferences.gitTool == 'cli' %}
1. Abre tu interfaz de línea de comandos favorita, a la que llamaremos shell a partir de ahora.
1. Clona este repositorio:
      ```shell
      git clone {{ thePayload.repository.clone_url }}
      ```
1. Navega al repositorio en tu shell:
      ```shell
      cd {{ thePayload.repository.name }}
      ```
1. Cambia a la rama de esta solicitud de extracción:
      ```shell
      git checkout add-headers
      ```
1. En tu editor de textos, abre el archivo `01-name.md`, en el directorio `_includes`. En la primera línea, sustituye el texto con tu nombre y añade una `#` antes del contenido para convertirlo en un encabezado H1.
1. Guarda el archivo. Cada vez que hagas algún cambio, es buena idea teclear `git status`. Deberías hacer esto después de que añadas archivos como preparados para confirmar, y después de confirmar cambios. 
1. Añade el archivo como preparado para confirmar:
      ```shell
      git add _includes/01-name.md
      ```
1. Confirma el cambio y añade un mensaje de confirmación:
      ```shell
      git commit -m "<TU MENSAJE>"
      ```
1. Sube tus nuevos cambios confirmados a GitHub:
      ```shell
      git push
      ```
{% elsif preferences.gitTool == 'vscode' %}
1. Descarga y abre [Visual Studio Code](https://code.visualstudio.com/Download) (referido como VS Code) si aún no lo tienes.
1. En VS Code, abre la Paleta de Comandos (o _Command Palette_) usando <kbd>Ctrl+Mayús+P</kbd> en Windows, o <kbd>Command ⌘+Mayús+P</kbd> en macOS. También puedes seguir [la documentación oficial de VS Code](https://code.visualstudio.com/docs/editor/versioncontrol#_cloning-a-repository) sobre clonar repositorios.
1. Escribe `git clone`y presiona <kbd>Enter</kbd>
      ![una captura de pantalla de VS Code con la Paleta de Comandos abierta](https://user-images.githubusercontent.com/16547949/53639288-bcf9ec80-3bf6-11e9-9d18-d97167168248.png)
1. Pega la URL del repositorio en la nueva ventana y presiona <kbd>Enter</kbd>:
      ```shell
      {{ thePayload.repository.clone_url }}
      ```
1. Selecciona la ubicación en el que quieres guardar el repositorio y haz clic en **Choose folder**. Después, abre la ubicación que seleccionaste (haciendo clic en **Open**).  
1. El directorio del repositiorio debería estar ahora abierto en tu proyecto de VS Code. Haz clic en `add-headers` en la parte inferior de la ventana de VS Code. Esto abrirá la Paleta de Comandos con todos los comandos relacionados a ramas de Git. 
      ![una captura de pantalla de las ramas de Git en VS Code](https://user-images.githubusercontent.com/16547949/53639606-adc76e80-3bf7-11e9-98ac-bd41ae2b40db.png)
1. En la ventana de edición, abre el archivo `01-name.md`, en el directorio `_includes`. En la primera línea, sustituye el texto con tu nombre y añade una `#` antes del contenido para convertirlo en un encabezado H1.
2. Guarda el archivo.
1. Para añadir tu nuevo archivo ve a la vista de Source Control y haz clic en el botón **+** a lado del archivo. También puedes seguir este paso con la [documentación oficial de VS Code](https://code.visualstudio.com/docs/editor/versioncontrol#_commit).
      ![una captura del botón de staging en la vista Source  Control](https://user-images.githubusercontent.com/16547949/53641057-d5b8d100-3bfb-11e9-9b69-53b0661cd5cd.png)
1. Haz una confirmación de cambios escribiendo un mensaje de confirmación en el campo de texto y después presionando<kbd>Ctrl+Enter</kbd> en Windows o <kbd>Comando ⌘+Enter</kbd> en macOS.
      ![una captura del mensaje de confirmación de cambios VS Code](https://user-images.githubusercontent.com/16547949/53641276-698a9d00-3bfc-11e9-9b3d-01680fd01d7c.png)
1. Haz clic en los puntos suspensivos (...) y selecciona **Pull, Push > Push**.```

{% else %}
1. En esta solicitud de extracción, haz clic en la pestaña **Files changed**.
1. En el extremo superior derecho de la vista de archivo, haz clic en el icono de **lápiz** ✏️ del archivo titulado `_includes/01-name.md`.
1. En la pestaña **Edit file**, añade una `#` antes del contenido para convertirlo en un encabezado H1. Puedes añadir más encabezados, usando entre uno y seis caracteres `#`.
1. Encima de tu nuevo contenido, haz clic en **Preview changes**.
1. En la parte inferior de la página, escribe un mensaje de confirmación breve y significativo que describa el cambio que has realizado en el archivo.
1. Haz clic en **Commit changes**.
{% endif %}

<hr>
<h3 align="center">Mira mi respuesta aquí debajo.</h3>
