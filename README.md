# Rainbow Cyberpunk Neon

<p align="center">
  <img src="https://img.shields.io/badge/VS%20Code-Theme-00f0ff?style=flat-square&logo=visualstudiocode&logoColor=white" alt="VS Code Theme" />
  <img src="https://img.shields.io/badge/Cursor-compatible-ff2bd6?style=flat-square" alt="Cursor" />
  <img src="https://img.shields.io/badge/license-MIT-c8ff00?style=flat-square" alt="MIT" />
  <img src="https://img.shields.io/badge/version-0.1.0-00ffff?style=flat-square" alt="0.1.0" />
</p>

Tema oscuro cyberpunk / cristal para **VS Code** y **Cursor**: lima, cyan, amarillo, rosa, naranja y rojo neón, con fondos púrpura translúcidos.

El paquete está preparado para **Visual Studio Marketplace** (`package.json` listo), pero **aún no está publicado**. Por ahora instálalo desde este repositorio o con un VSIX local (véase abajo).

## Paleta (prioridad visual)

1. Lima neón (chartreuse) `#c8ff00`
2. Cyan neón `#00ffff`
3. Amarillo neón `#ffff00`
4. Rosa neón `#ff00d4`
5. Naranja neón `#ff6a00`
6. Rojo neón `#ff3131`

## Captura

![Rainbow Cyberpunk Neon](./media/screenshot-cyberpunk.png)

## Instalación desde GitHub (sin Marketplace)

### Opción A: clonar en la carpeta de extensiones (Cursor)

Carpeta de extensiones de Cursor según SO:

| SO | Ruta |
| --- | --- |
| **Linux** | `~/.cursor/extensions` |
| **macOS** | `~/.cursor/extensions` |
| **Windows** | `%USERPROFILE%\.cursor\extensions` |

```bash
# Linux / macOS
cd ~/.cursor/extensions
git clone https://github.com/xyz-rainbow/rainbow-cyberpunk-neon-theme.git

# Windows (PowerShell)
cd $env:USERPROFILE\.cursor\extensions
git clone https://github.com/xyz-rainbow/rainbow-cyberpunk-neon-theme.git
```

Reinicia Cursor. Luego `Ctrl+Shift+P` → **Preferences: Color Theme** → **Rainbow Cyberpunk Neon**.

### Opción B: VSIX local

En el clon del repo:

```bash
cd rainbow-cyberpunk-neon-theme
npx @vscode/vsce package
VERSION=$(node -p "require('./package.json').version")
```

Instala el VSIX generado (`rainbow-cyberpunk-neon-theme-${VERSION}.vsix`):

```bash
# VS Code
code --install-extension "rainbow-cyberpunk-neon-theme-${VERSION}.vsix"

# Cursor (CLI `cursor`)
cursor --install-extension "rainbow-cyberpunk-neon-theme-${VERSION}.vsix"
```

En Cursor también puedes instalar el `.vsix` desde la paleta de comandos (**Extensions: Install from VSIX...**) si tu build lo permite.

### Opción C: VS Code (extensión en carpeta de extensiones)

| SO | Ruta |
| --- | --- |
| **Linux** | `~/.vscode/extensions` |
| **macOS** | `~/.vscode/extensions` |
| **Windows** | `%USERPROFILE%\.vscode\extensions` |

```bash
# Linux / macOS
cd ~/.vscode/extensions
git clone https://github.com/xyz-rainbow/rainbow-cyberpunk-neon-theme.git

# Windows (PowerShell)
cd $env:USERPROFILE\.vscode\extensions
git clone https://github.com/xyz-rainbow/rainbow-cyberpunk-neon-theme.git
```

## Personalización extra (Cursor / VS Code)

Puedes refinar peso de fuente en `settings.json`:

```json
"editor.fontWeight": "500",
"terminal.integrated.fontWeight": "500"
```

## Autor

- GitHub: **xyz-rainbow**
- Correo: `rainbow@rainbowtechnology.xyz`

## Sponsor this project

Si te gusta el tema, puedes apoyar el proyecto:

- [Buy Me a Coffee](https://buymeacoffee.com/xyzclouds)
- [Ko-fi](https://ko-fi.com/xyzclouds)
- [Patreon](https://patreon.com/xyzclouds)
- [PayPal](https://paypal.me/rainbowkolors)

MIT License — ver `LICENSE`.
