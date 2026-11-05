<p align="center">
  <a href="https://getartcraft.com/">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="docs/brand/artcraft-logo-white.svg">
      <img alt="ArtCraft" src="docs/brand/artcraft-logo.svg" width="200">
    </picture>
  </a>
</p>

<p align="center">
  <img src="assets/app-icon/hicolor/256x256/apps/ai.storyteller.craft-anything.png" width="128" height="128" alt="Icono de Craft Anything: un cuervo grabado sobre una placa azul">
</p>

<h1 align="center">Craft Anything</h1>

<p align="center">
  <a href="README.md">English</a> · <b>Español</b> · <a href="README.ja.md">日本語</a> · <a href="README.zh.md">简体中文</a> · <a href="README.ko.md">한국어</a>
</p>

<p align="center">
  <b>Descubre cómo funciona cualquier sitio web, aplicación o juego y deja que la IA construya tu propia versión; un motor de sala limpia, de código abierto y escrito íntegramente en Rust.</b><br>
  Señala un objetivo, explica lo que quieres y la aplicación estudiará el original con herramientas de inspección reales;<br>
  después, un agente de programación creará un proyecto nuevo, lo comparará con el original y lo perfeccionará.
</p>

<p align="center">
  <img alt="100 % Rust" src="https://img.shields.io/badge/100%25-Rust-b7410e?style=flat-square&logo=rust">
  <img alt="macOS · Windows · Linux · FreeBSD · Web" src="https://img.shields.io/badge/macOS%20%C2%B7%20Windows%20%C2%B7%20Linux%20%C2%B7%20FreeBSD%20%C2%B7%20Web-native-2d81ff?style=flat-square">
  <img alt="Licencia: MIT OR Apache-2.0" src="https://img.shields.io/badge/license-MIT%20%2F%20Apache--2.0-3a3a3a?style=flat-square">
  <img alt="Estado: alfa temprana" src="https://img.shields.io/badge/status-early%20alpha-d69e2e?style=flat-square">
</p>

<p align="center">
  <a href="https://discord.gg/artcraft"><img alt="Únete a la comunidad de ArtCraft en Discord" src="https://img.shields.io/badge/Join%20us%20on%20Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white" height="40"></a>
</p>

<p align="center">
  <a href="#descargas"><b>Descargar Craft Anything</b></a> ·
  <a href="https://getartcraft.com/">ArtCraft</a> ·
  <a href="https://getartcraft.com/apps">Todas las aplicaciones Crafting</a>
</p>

<br>

<p align="center">
  <img src="docs/images/project-website.png" alt="Un proyecto de sitio web en Craft Anything: la comprobación enumera lo que aún no coincide y el grado de similitud de cada página; el constructor indica que su versión está lista; una tarjeta solicita aprobación antes de ejecutar un comando; y el plan muestra dos de cuatro pasos completados" width="100%">
  <br>
  <sub>Un proyecto de sitio web: cada comprobación indica cuánto se parece la compilación; tú apruebas cualquier acción que quede fuera de las reglas; y el plan muestra lo que falta.</sub>
</p>

> [!NOTE]
> **ArtCraft es una comunidad de artistas de todos los ámbitos.** Pintores, fotógrafos,
> cineastas, ilustradores, diseñadores, animadores, aficionados y personas que tomaron un lápiz
> por primera vez la semana pasada. Si creas cosas, eres parte de la comunidad. **[Ven a saludar en Discord](https://discord.gg/artcraft).**

<p align="center">
  <a href="#cómo-funciona">Cómo funciona</a> ·
  <a href="#dos-formas-de-usarlo">Dos formas de usarlo</a> ·
  <a href="#ia">IA</a> ·
  <a href="#diseñado-para-agentes">Agentes</a> ·
  <a href="#bajo-el-capó">Bajo el capó</a> ·
  <a href="#primeros-pasos">Primeros pasos</a> ·
  <a href="#estado">Estado</a> ·
  <a href="#descargas">Descargas</a> ·
  <a href="https://discord.gg/artcraft">Discord</a>
</p>

<br>

<table>
  <tr>
    <td width="25%" valign="top">
      <h3>🔍 Estudia cualquier cosa</h3>
      Sitios web, aplicaciones de escritorio y móviles, juegos y archivos: herramientas de inspección reales descubren cómo están hechos y qué hacen, con las evidencias que respaldan cada respuesta.
    </td>
    <td width="25%" valign="top">
      <h3>🛠️ Construye tu propia versión</h3>
      Explica lo que quieres ("Recrea este sitio web", "Recrea la mecánica de este juego en Rust") y un agente de programación creará un proyecto nuevo con la tecnología que solicites.
    </td>
    <td width="25%" valign="top">
      <h3>✅ Comprobado, no supuesto</h3>
      Cada compilación se compara con el original (páginas en tres anchos de pantalla, la autoprueba de un juego o las ejecuciones de una aplicación) y se perfecciona hasta acercarse al resultado esperado.
    </td>
    <td width="25%" valign="top">
      <h3>🤖 Preparado para agentes</h3>
      320 herramientas, cada una disponible como comando de CLI y herramienta MCP, para que cualquier agente pueda controlar el mismo motor que usa la aplicación. No se necesita IA para inspeccionar.
    </td>
  </tr>
</table>

<br>

## Cómo funciona

Señala un objetivo a Craft Anything, explica lo que quieres y pulsa Iniciar. El proceso tiene cuatro
pasos y te consulta con palabras sencillas cuando una decisión depende de ti:

1. **Estudiar:** inspecciona el original: sus páginas en distintos anchos, su código, sus archivos y su funcionamiento.
2. **Construir:** un agente de programación crea un proyecto nuevo en el lenguaje, framework o motor
   que indiques en la solicitud (o elige una opción razonable de forma predeterminada).
3. **Comprobar:** compara la compilación con el original y enumera lo que todavía no coincide.
4. **Listo:** abre, juega o previsualiza el resultado; también puedes pedir cambios para que lo perfeccione.

<table>
  <tr>
    <td width="50%" valign="top">
      <img src="docs/images/make.png" alt="Pantalla Crear: elige un sitio web, una aplicación o un juego para recrearlo; escribe la dirección; elige Sala limpia o Profundo; explica lo que quieres y pulsa Iniciar" width="100%"><br>
      <sub><b>Crear:</b> elige qué recrear, explica lo que quieres y pulsa Iniciar.</sub>
    </td>
    <td width="50%" valign="top">
      <img src="docs/images/project-game.png" alt="Proyecto terminado de un juego de la serpiente, con todos los pasos completos y un botón para jugar" width="100%"><br>
      <sub><b>Listo:</b> juega o solicita cambios debajo.</sub>
    </td>
  </tr>
</table>

## Dos formas de usarlo

- **Simple** (predeterminada): «¿Qué quieres crear?». Elige un sitio web, una aplicación o un juego,
  descríbelo y pulsa Iniciar. La página del proyecto muestra los cuatro pasos (Estudiar → Construir →
  Comprobar → Listo), explica con palabras sencillas lo que hace el agente, presenta tarjetas de
  preguntas y aprobaciones, indica cuánto se parece el resultado e incluye botones para abrirlo o
  abrir su carpeta. Solicita cambios en el cuadro inferior. «Solo mirar dentro» abre un objetivo
  para hacer preguntas sin construir nada (en modo Profundo).
- **Avanzada:** el banco de trabajo completo: todas las herramientas (Ctrl/Cmd+K), funciones,
  cadenas, seudocódigo C, desensamblado, hexadecimal, grafos de llamadas, evidencias, incógnitas,
  trabajos, registros y la consola del agente.

Ambos modos utilizan el mismo motor.

## Sala limpia o Profundo

- **Sala limpia** (predeterminada): no se lee nada del interior del original: ni su código, ni sus
  archivos, ni el código fuente de sus páginas. Craft Anything trabaja con lo que puedes ver: las
  imágenes que añades; el sitio web tal como lo ve un visitante (capturas, texto visible, diseño
  medido, colores, tipografías, espaciado y menús abiertos); y, cuando lo autorizas, una imagen de
  la ventana de la aplicación. Las herramientas que mirarían dentro se rechazan e indican cómo
  activar el modo Profundo.
- **Profundo:** utiliza todas las herramientas para tu uso privado. Los motores incorporados leen
  el código y los archivos de un programa (y también Ghidra, si está instalado); se lee el
  JavaScript de un sitio web y se observa su página inicial; y el constructor puede usar toda esa
  información.

Sala limpia es una regla sobre lo que Craft Anything ofrece y rechaza. No es un entorno aislado del
sistema operativo: no aísla el equipo. El agente de programación que ejecutes seguirá actuando con
tus permisos; lo que pueda leer, escribir o ejecutar dependerá de sus propios permisos. Las
herramientas del agente que Craft Anything puede rechazar varían según el agente; para las
herramientas de Claude Code en chats y preguntas, consulta
[`docs/claude-code.md`](docs/claude-code.md).

Cambia el modo desde la barra de título o desde Ajustes, con `settings_set deep_mode true`, o para
una sola ejecución de CLI con `--deep` (o `--clean-room`).

<p align="center">
  <img src="docs/images/workbench.png" alt="Banco de trabajo Avanzado: una lista de funciones, el seudocódigo C de la función seleccionada, el agente respondiendo una pregunta mediante una herramienta y el registro de evidencias" width="100%">
  <br>
  <sub><b>Avanzado:</b> funciones, seudocódigo C, el agente y las evidencias que respaldan cada respuesta.</sub>
</p>

## IA

La construcción necesita un agente de programación en tu equipo. **Claude Code** es el primer
agente compatible: Craft Anything ejecuta tu propio programa `claude`, sin modificarlo, y utiliza
tu propia sesión; Craft Anything nunca ve ni gestiona tu cuenta. Su uso se rige por tu propio
acuerdo con Anthropic. Consulta [docs/claude-code.md](docs/claude-code.md) para saber cómo y por
qué. Existe un adaptador para Codex, pero todavía no se ha verificado en una instalación real.
**GitHub Copilot** puede utilizar tu CLI de Copilot instalada mediante ACP: inicia sesión por
separado con `copilot login`. Otros agentes compatibles con ACP (Gemini CLI, Qwen Code, opencode,
goose, Hermes y Maki) pueden seleccionarse para cada backend; de ellos, solo Maki se ha ejecutado
en vivo. Anthropic, OpenAI, OpenRouter y los servidores locales compatibles con OpenAI están
disponibles para preguntas y análisis (Ajustes → IA).

## Diseñado para agentes

Cada herramienta también es un subcomando de CLI y una herramienta MCP, por lo que un agente puede
estudiar un objetivo o ejecutar una reconstrucción completa sin la aplicación:

```sh
craft-anything-cli commands                                   # todas las herramientas, por conjunto
craft-anything-cli mcp                                        # las ofrece a cualquier cliente MCP
craft-anything-cli rebuild https://example.com "Recrea este sitio web"
```

Los resultados son registros de evidencias con su confianza, cobertura y limitaciones. Los
resultados grandes devuelven primero un resumen y se consultan por páginas mediante
`core_evidence_browse`. `craft-anything-cli setup` conecta Craft Anything con aplicaciones de
agentes de programación.

## Bajo el capó

Un motor de ingeniería inversa escrito íntegramente en Rust, con 320 herramientas (300 en el motor
y el resto en las capas de IA y configuración) para programas nativos, .NET, Java, Android, Apple,
Electron/JavaScript, sitios web, firmware, capturas de paquetes, bases de datos y archivos de
juegos. Sus propios decodificadores, desensamblador y descompilador funcionan sin programas
externos; el modo Profundo los utiliza todos y añade Ghidra cuando está instalado. El motor impulsa
la aplicación de escritorio (egui), la CLI y el servidor MCP, y algunas partes se ejecutan en el
navegador como WebAssembly. La lista completa está en [docs/tools.md](docs/tools.md).

## Primeros pasos

Requiere Rust **1.97 o posterior** (una dependencia lo necesita; ejecuta `rustup update`). En Debian
o Ubuntu, la aplicación de escritorio también necesita:

```sh
sudo apt-get install libxkbcommon-dev libwayland-dev libx11-dev libxrandr-dev libxi-dev libgl1-mesa-dev libgtk-3-dev
```

Después:

```sh
git clone https://github.com/storytold/craft-anything && cd craft-anything
cargo run --release -p craft-anything                # aplicación de escritorio
cargo install --path apps/craft-anything-cli         # instala la CLI como `craft-anything-cli`
craft-anything-cli doctor                            # comprueba la instalación, los agentes y los motores
```

Para construir se necesita un agente de programación con una sesión iniciada en el equipo
(consulta [IA](#ia)); `doctor` indica qué falta. Reconstruye desde la línea de comandos (las
preguntas se hacen en el terminal):

```sh
craft-anything-cli rebuild https://example.com "Recrea este sitio web"
craft-anything-cli rebuild - "Un juego de la serpiente en Rust" --rounds 1
craft-anything-cli rebuild https://example.com "Haz que el encabezado sea azul" --continue-in "<carpeta del proyecto>"
craft-anything-cli rebuild - "Añade un formulario de contacto" --project-folder "<tu carpeta>" --existing edit
```

Los proyectos nuevos se guardan en `Documents/Craft Anything` (puedes cambiarlo en Ajustes →
General). Cada carpeta de proyecto contiene `craft.json` (la solicitud, el objetivo, el estado y el
historial), `capture/` (lo registrado del objetivo), `app/` (el proyecto generado), `checks/`
(cada comparación con el original), `investigation.cany/` (las evidencias) e `inbox/` (las
preguntas pendientes).

También puedes iniciar un proyecto en una carpeta que elijas (Elegir una carpeta… bajo Iniciar, o
`--project-folder`). Si ya contiene archivos, debes indicar qué son: la propia aplicación, que el
constructor editará directamente; o material de partida, en cuyo caso la aplicación se creará en
`app/` junto a esos archivos (Ajustes → General puede recordar la respuesta). Ajustes → General
también enumera proyectos de otras carpetas; al quitar uno solo se elimina de la lista.

## Estado

> [!IMPORTANT]
> **Estado:** Craft Anything se encuentra en una fase alfa temprana. Lo que funciona hoy, lo que
> está parcialmente implementado y lo que viene después:
>
> - **Funciona hoy:** la aplicación de escritorio (Simple y Avanzada), la CLI y el servidor MCP;
>   el flujo Estudiar → Construir → Comprobar → Perfeccionar para sitios web, aplicaciones y juegos
>   con Claude Code como constructor; comprobaciones de sitios web en tres anchos de pantalla;
>   reconstrucción de juegos en Unity, Unreal o Godot; modo Profundo con Ghidra; imágenes y modelos
>   3D generados (opcional, con tu propia clave de fal.ai); y complementos (servidores MCP y
>   componentes WASM en compilaciones con la opción `wasm-plugins`).
> - **Parcialmente disponible:** construcción con claves de API y otros agentes de programación
>   (implementada, pero aún no ejecutada en vivo), comprobaciones de comportamiento para
>   aplicaciones y juegos, y algunas herramientas de motor probadas únicamente con sustitutos.
> - **Publicado:** hay versiones públicas con instaladores para Windows, macOS, Linux y FreeBSD en
>   la [página de versiones](https://github.com/storytold/craft-anything/releases); siguen siendo alfa.
> - **A continuación:** el nivel administrado.
>
> [docs/STATUS.md](docs/STATUS.md) contiene los detalles y explica cómo se comprobó cada parte;
> [docs/tool-status.md](docs/tool-status.md), la lista de comprobación herramienta por herramienta;
> y [docs/ROADMAP.md](docs/ROADMAP.md), el plan detallado. Abre una incidencia o cuéntanos qué falló
> en [Discord](https://discord.gg/artcraft).

**Uso responsable.** Utiliza Craft Anything con software de tu propiedad o que tengas permiso para
examinar. Nunca elude DRM, inicios de sesión ni sistemas antitrampas. Las reconstrucciones recrean
el diseño, el estilo y el comportamiento a partir de evidencias; se indica al agente que no copie
logotipos, fotografías ni textos salvo que confirmes que son tuyos o que tienes permiso.

**Instalar dependencias ejecuta código.** Cuando un constructor instala las dependencias de un
proyecto, los comandos se ejecutan en tu equipo y los paquetes pueden ejecutar código durante la
instalación. npm ejecuta de forma predeterminada los scripts de instalación de cada paquete; los
scripts de compilación de Rust y los paquetes fuente de Python ejecutan sus propios procesos de
configuración. Craft Anything pide permiso antes de ejecutar un tipo de comando que todavía no haya
visto en el proyecto (`npm`, `cargo`…). Elegir «permitir siempre» para `npm` permite que todos los
comandos npm posteriores se ejecuten sin preguntar: hazlo únicamente en proyectos cuyas
dependencias sean de confianza. Para instalar paquetes npm sin ejecutar sus scripts de instalación,
utiliza `npm install --ignore-scripts`.

## Descargas

En GitHub, la [versión más reciente](https://github.com/storytold/craft-anything/releases/latest)
incluye todas las compilaciones que aparecen a continuación, y [todas las versiones](https://github.com/storytold/craft-anything/releases)
contiene las versiones anteriores y sus notas. `<ver>` representa el número de versión en los
nombres de archivo, y `SHA256SUMS.txt` contiene una suma de comprobación para cada archivo.

### Windows

| Compilación | Instalador | Portátil |
|---|---|---|
| x64 (Intel/AMD de 64 bits) | `craft-anything-<ver>-windows-x64.msi` | `craft-anything-<ver>-windows-x64-portable.zip` |
| arm64 (Snapdragon y otros equipos ARM) | `craft-anything-<ver>-windows-arm64.msi` | `craft-anything-<ver>-windows-arm64-portable.zip` |
| x86 (32 bits) | `craft-anything-<ver>-windows-x86.msi` | `craft-anything-<ver>-windows-x86-portable.zip` |

Los instaladores y ejecutables están firmados digitalmente. El archivo ZIP portátil conserva su
configuración junto a la aplicación.

### macOS

| Compilación | Archivo | Notas |
|---|---|---|
| Aplicación universal (Apple silicon + Intel) | `craft-anything-<ver>-macos-universal.dmg` | Firmada y notarizada |
| Herramienta de línea de comandos universal | `craft-anything-cli-<ver>-macos-universal.zip` | Firmada y notarizada; consulta la información siguiente si macOS la bloquea |

Las versiones posteriores a 0.2.0 incluyen la herramienta de línea de comandos en la aplicación,
por lo que las compilaciones no necesitan el ZIP independiente. Solo lo necesitas para utilizar la
línea de comandos sin la aplicación.

La descarga del ZIP desde un navegador puede detenerse con «Apple no pudo verificar
craft-anything-cli» (un programa independiente no puede llevar consigo su notarización, por lo que
macOS debe consultarla en línea). Las descargas desde el terminal no se comprueban de esta manera;
utiliza lo siguiente:

```sh
ver=0.2.0   # cámbialo por la versión que quieras
curl -fLO "https://github.com/storytold/craft-anything/releases/download/v$ver/craft-anything-cli-$ver-macos-universal.zip"
ditto -x -k "craft-anything-cli-$ver-macos-universal.zip" .
mkdir -p ~/.local/bin
mv "craft-anything-cli-$ver-macos-universal/craft-anything-cli" ~/.local/bin/
~/.local/bin/craft-anything-cli --version
```

Para ejecutarla simplemente como `craft-anything-cli`, añade `~/.local/bin` a tu `PATH`.

Si ya tienes una copia bloqueada, pulsa OK (no Mover a la papelera) y ejecuta
`xattr -d com.apple.quarantine <ruta a craft-anything-cli>`, o autorízala en Ajustes del Sistema →
Privacidad y seguridad → Abrir igualmente.

#### Comprobar que una descarga para Mac está firmada y notarizada

Cada versión para Mac está firmada con un certificado Developer ID y notarizada por Apple. Para
comprobar una descarga, ejecuta lo siguiente en el Terminal (sustituye `<ver>` por la versión y las
rutas por las tuyas):

```sh
# La imagen de disco: "accepted" y "source=Notarized Developer ID" indican que superó la comprobación
spctl --assess --type open --context context:primary-signature -v "craft-anything-<ver>-macos-universal.dmg"
# El ticket de notarización está adjunto: muestra "The validate action worked!"
xcrun stapler validate "craft-anything-<ver>-macos-universal.dmg"

# La aplicación, después de abrir la imagen de disco: la firma debe verificarse
codesign --verify --deep --strict --verbose=2 "/Volumes/<nombre de la imagen de disco>/Craft Anything.app"
spctl --assess --type execute --verbose "/Volumes/<nombre de la imagen de disco>/Craft Anything.app"

# Herramienta de línea de comandos: un programa independiente no puede llevar un ticket, así que macOS lo comprueba en línea
codesign --verify --strict --verbose=2 ~/.local/bin/craft-anything-cli
codesign -dv --verbose=4 ~/.local/bin/craft-anything-cli 2>&1 | grep Authority
```

Las líneas `Authority` deben mencionar un certificado «Developer ID Application». Si alguna
comprobación falla, no ejecutes el archivo; informa del problema e incluye la salida y la etiqueta
de la versión.

### Linux

| Formato | x86_64 | aarch64 (ARM64) | Notas |
|---|---|---|---|
| AppImage | `craft-anything-<ver>-linux-x86_64.AppImage` | `craft-anything-<ver>-linux-aarch64.AppImage` | Funciona en cualquier distribución; se actualiza mediante [AppImageUpdate](https://github.com/AppImageCommunity/AppImageUpdate) (archivos `.zsync`) |
| Flatpak | `craft-anything-<ver>-linux-x86_64.flatpak` | `craft-anything-<ver>-linux-aarch64.flatpak` | Aislado; `flatpak install --user <archivo>` |
| Debian/Ubuntu | `craft-anything-<ver>-linux-x86_64.deb` | `craft-anything-<ver>-linux-aarch64.deb` | |
| Fedora/RHEL/openSUSE | `craft-anything-<ver>-linux-x86_64.rpm` | `craft-anything-<ver>-linux-aarch64.rpm` | |
| Tarball | `craft-anything-<ver>-linux-x86_64.tar.gz` | `craft-anything-<ver>-linux-aarch64.tar.gz` | Se puede extraer en cualquier lugar |

RISC-V (riscv64): `craft-anything-<ver>-linux-riscv64.tar.gz`, solo en formato tarball.

La AppImage también contiene la CLI: ejecuta `<AppImage> --cli <comando>` (por ejemplo,
`<AppImage> --cli mcp` para un cliente MCP), o crea un enlace a la AppImage llamado
`craft-anything-cli` y ejecútalo.

### FreeBSD

| Compilación | Archivo |
|---|---|
| x86_64 | `craft-anything-<ver>-freebsd-x86_64.tar.gz` |

### Web (WebAssembly)

| Compilación | Archivo | Notas |
|---|---|---|
| Visor para navegador | `craft-anything-web-<ver>.zip` | Identifica un archivo dentro del navegador (el archivo nunca sale de él); aloja la carpeta en cualquier servidor web estático ([packaging/web/README.md](packaging/web/README.md)) |

<br>

<p align="center">
  <a href="https://discord.gg/artcraft"><img alt="Únete a la comunidad de ArtCraft en Discord" src="https://img.shields.io/badge/Join%20us%20on%20Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white" height="40"></a>
</p>

<h3 align="center">Ven a crear con nosotros</h3>

<p align="center">
  Nuestro Discord es el lugar donde se reúnen artistas de todo tipo: personas que pintan,
  fotografían, dibujan, editan películas, trabajan con tipografía y quienes todavía están
  descubriendo qué les gusta crear. Comparte tu trabajo, pide ayuda, cuéntanos qué está roto o qué
  te gustaría que pudieran hacer estas herramientas. Sin importar tu disciplina ni el tiempo que
  lleves practicándola, aquí eres bienvenido.
</p>

<p align="center">
  <a href="https://discord.gg/artcraft"><b>discord.gg/artcraft</b></a> ·
  <a href="https://getartcraft.com/">getartcraft.com</a> ·
  <a href="https://getartcraft.com/apps">Las aplicaciones Crafting</a> ·
  <a href="https://github.com/storytold/craft-anything">Craft Anything</a>
</p>

---

## El conjunto de aplicaciones Craft

| | Aplicación | Para qué sirve | Código | Más información |
|:-:|---|---|---|---|
| <img src="https://raw.githubusercontent.com/storytold/photocraft/main/assets/app-icon/hicolor/64x64/apps/ai.storyteller.photocraft.png" alt="" width="32" height="32"> | **PhotoCraft** | Edición de imágenes: capas, máscaras, texto y archivos PSD reales | [GitHub](https://github.com/storytold/photocraft) | [Sitio web](https://getartcraft.com/apps/photocraft) |
| <img src="https://raw.githubusercontent.com/storytold/vectorcraft/main/assets/app-icon/hicolor/64x64/apps/ai.storyteller.vectorcraft.png" alt="" width="32" height="32"> | **VectorCraft** | Ilustración vectorial | [GitHub](https://github.com/storytold/vectorcraft) | [Sitio web](https://getartcraft.com/apps/vectorcraft) |
| <img src="https://raw.githubusercontent.com/storytold/filmcraft/main/assets/app-icon/hicolor/64x64/apps/ai.storyteller.filmcraft.png" alt="" width="32" height="32"> | **FilmCraft** | Edición de video, color y sonido | [GitHub](https://github.com/storytold/filmcraft) | [Sitio web](https://getartcraft.com/apps/filmcraft) |
| <img src="https://raw.githubusercontent.com/storytold/lightcraft/main/assets/app-icon/hicolor/64x64/apps/ai.storyteller.lightcraft.png" alt="" width="32" height="32"> | **LightCraft** | Biblioteca fotográfica y revelado RAW | [GitHub](https://github.com/storytold/lightcraft) | [Sitio web](https://getartcraft.com/apps/lightcraft) |
| <img src="https://raw.githubusercontent.com/storytold/pdfcraft/main/assets/app-icon/hicolor/64x64/apps/ai.storyteller.pdfcraft.png" alt="" width="32" height="32"> | **PdfCraft** | Lectura, organización y protección de archivos PDF | [GitHub](https://github.com/storytold/pdfcraft) | [Sitio web](https://getartcraft.com/apps/pdfcraft) |
| <img src="https://raw.githubusercontent.com/storytold/effectcraft/main/assets/app-icon/hicolor/64x64/apps/ai.storyteller.effectcraft.png" alt="" width="32" height="32"> | **EffectCraft** | Gráficos animados y efectos visuales | [GitHub](https://github.com/storytold/effectcraft) | [Sitio web](https://getartcraft.com/apps/effectcraft) |
| <img src="https://raw.githubusercontent.com/storytold/designcraft/main/assets/app-icon/hicolor/64x64/apps/ai.storyteller.designcraft.png" alt="" width="32" height="32"> | **DesignCraft** | Maquetación y publicación | [GitHub](https://github.com/storytold/designcraft) | [Sitio web](https://getartcraft.com/apps/designcraft) |
| <img src="https://raw.githubusercontent.com/storytold/figcraft/main/assets/app-icon/hicolor/64x64/apps/ai.storyteller.figcraft.png" alt="" width="32" height="32"> | **FigCraft** | Diseño de interfaces y creación de prototipos | [GitHub](https://github.com/storytold/figcraft) | [Sitio web](https://getartcraft.com/apps/figcraft) |
| <img src="https://raw.githubusercontent.com/storytold/wordcraft/main/assets/app-icon/hicolor/64x64/apps/ai.storyteller.wordcraft.png" alt="" width="32" height="32"> | **WordCraft** | Procesamiento de textos y documentos | [GitHub](https://github.com/storytold/wordcraft) | [Sitio web](https://getartcraft.com/apps/wordcraft) |
| <img src="https://raw.githubusercontent.com/storytold/soundcraft/main/assets/app-icon/hicolor/64x64/apps/ai.storyteller.soundcraft.png" alt="" width="32" height="32"> | **SoundCraft** | Grabación y edición de audio | [GitHub](https://github.com/storytold/soundcraft) | [Sitio web](https://getartcraft.com/apps/soundcraft) |
| <img src="https://raw.githubusercontent.com/storytold/deckcraft/main/assets/app-icon/hicolor/64x64/apps/ai.storyteller.deckcraft.png" alt="" width="32" height="32"> | **DeckCraft** | Presentaciones y diapositivas | [GitHub](https://github.com/storytold/deckcraft) | [Sitio web](https://getartcraft.com/apps/deckcraft) |
| <img src="https://raw.githubusercontent.com/storytold/cadcraft/main/assets/app-icon/hicolor/64x64/apps/ai.storyteller.cadcraft.png" alt="" width="32" height="32"> | **CADCraft** | Diseño asistido por ordenador | [GitHub](https://github.com/storytold/cadcraft) | [Sitio web](https://getartcraft.com/apps/cadcraft) |
| <img src="https://raw.githubusercontent.com/storytold/gridcraft/main/assets/app-icon/hicolor/64x64/apps/ai.storyteller.gridcraft.png" alt="" width="32" height="32"> | **GridCraft** | Hojas de cálculo y datos | [GitHub](https://github.com/storytold/gridcraft) | [Sitio web](https://getartcraft.com/apps/gridcraft) |
| <img src="https://raw.githubusercontent.com/storytold/texturecraft/main/assets/app-icon/hicolor/64x64/apps/ai.storyteller.texturecraft.png" alt="" width="32" height="32"> | **TextureCraft** | Pintura de texturas 3D | [GitHub](https://github.com/storytold/texturecraft) | [Sitio web](https://getartcraft.com/apps/texturecraft) |
| <img src="https://raw.githubusercontent.com/storytold/craft-anything/main/assets/app-icon/hicolor/64x64/apps/ai.storyteller.craft-anything.png" alt="" width="32" height="32"> | **Craft Anything** | Descubre cómo funciona cualquier software y crea tu propia versión | [GitHub](https://github.com/storytold/craft-anything) | [Sitio web](https://getartcraft.com/apps/craft-anything) |
| <img src="https://raw.githubusercontent.com/tangency-labs/solidcraft/main/assets/icons/app/linux/exports/hicolor/64x64/apps/io.tangencylabs.solidcraft.png" alt="" width="32" height="32"> | **SolidCraft** | CAD 3D paramétrico de Tangency Labs (aplicación de la comunidad) | [GitHub](https://github.com/tangency-labs/solidcraft) | |


## Licencia y créditos

Craft Anything tiene licencia dual [MIT](LICENSE-MIT) o [Apache-2.0](LICENSE-APACHE), a tu elección.
Copyright (c) 2026 ArtCraft Team y las personas que contribuyen a Craft Anything. Los avisos
obligatorios están en [NOTICE](NOTICE).

Las tipografías, iconos, imágenes y demás recursos incluidos conservan sus propias licencias
abiertas. Cada recurso aparece con su autoría, fuente y licencia en
[ATTRIBUTION.md](ATTRIBUTION.md).

Las capturas muestran proyectos de ejemplo creados para ellas: example.com, un juego de la
serpiente y un pequeño programa de calculadora.

El nombre, la marca denominativa y los logotipos de ArtCraft en [`docs/brand/`](docs/brand/) son
marcas comerciales de ArtCraft Team y no están cubiertos por esta licencia. Solo pueden utilizarse
sin modificaciones y como parte de este repositorio y de Craft Anything, de acuerdo con
[`docs/brand/LICENSE-brand.txt`](docs/brand/LICENSE-brand.txt). Los forks y las versiones
modificadas deben eliminarlos.

<p align="center">
  <a href="https://getartcraft.com/"><img alt="ArtCraft" src="docs/brand/artcraft-mark.svg" width="28"></a><br>
  <sub>Creado por el equipo y la comunidad de <a href="https://getartcraft.com/">ArtCraft</a>.</sub>
</p>
