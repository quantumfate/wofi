<h3 align="center">
 <img src="https://raw.githubusercontent.com/catppuccin/catppuccin/main/assets/logos/exports/1544x1544_circle.png" width="100" alt="Logo"/><br/>
 <img src="https://raw.githubusercontent.com/catppuccin/catppuccin/main/assets/misc/transparent.png" height="30" width="0px"/>
 Catppuccin for <a href="https://hg.sr.ht/~scoopta/wofi">Wofi</a>
 <img src="https://raw.githubusercontent.com/catppuccin/catppuccin/main/assets/misc/transparent.png" height="30" width="0px"/>
</h3>

<p align="center">
 <a href="https://github.com/quantumfate/wofi/stargazers"><img src="https://img.shields.io/github/stars/catppuccin/template?colorA=363a4f&colorB=b7bdf8&style=for-the-badge"></a>
 <a href="https://github.com/quantumfate/wofi/issues"><img src="https://img.shields.io/github/issues/catppuccin/template?colorA=363a4f&colorB=f5a97f&style=for-the-badge"></a>
 <a href="https://github.com/quantumfate/wofi/contributors"><img src="https://img.shields.io/github/contributors/catppuccin/template?colorA=363a4f&colorB=a6da95&style=for-the-badge"></a>
</p>

<p align="center">
 <img src="https://raw.githubusercontent.com/quantumfate/wofi/main/assets/preview.webp"/>
</p>

## Previews

<details>
<summary>🌻 Latte</summary>
<img src="https://raw.githubusercontent.com/quantumfate/wofi/main/assets/latte.webp"/>
</details>
<details>
<summary>🪴 Frappé</summary>
<img src="https://raw.githubusercontent.com/quantumfate/wofi/main/assets/frappe.webp"/>
</details>
<details>
<summary>🌺 Macchiato</summary>
<img src="https://raw.githubusercontent.com/quantumfate/wofi/main/assets/macchiato.webp"/>
</details>
<details>
<summary>🌿 Mocha</summary>
<img src="https://raw.githubusercontent.com/quantumfate/wofi/main/assets/mocha.webp"/>
</details>

## Usage

1. Clone this repository locally to your desired location. Typically something like `~/.config/`
2. Launch Wofi with your desired flavor (e.g. `latte`, `frappe`, `macchiato` or `mocha`).

```bash
wofi --conf <your-path-to-wofi>/config --style <your-path-to-wofi>/<flavor>/style.css

```

I'm personally using a bash script:

```bash
#!/usr/bin/env bash

CONFIG="$HOME/.config/hypr/wofi/config/config"
STYLE="$HOME/.config/hypr/wofi/src/mocha/style.css"

if [[ ! $(pidof wofi) ]]; then
    wofi --conf "${CONFIG}" --style "${STYLE}"
else
    pkill wofi
fi
```

- Q: **_"Which flavor of CSS is supported."_**\
 A: [GTK CSS](https://docs.gtk.org/gtk3/). Note that hsl-colors are not supported.

- Q: **_"Where can I find CSS targets for theme customization."_**\
 A: On the [Wofi page](https://hg.sr.ht/~scoopta/wofi) and on the [man page](https://man.archlinux.org/man/wofi.7.en).

- Q: **_"My CSS imports are not working."_**\
 A: Please read the [Wofi configuration](https://man.archlinux.org/man/wofi.5.en#CONFIG_OPTIONS) options. Especially in regards to `style` and `stylesheet`. We avoid import statements for simplicity.

## 💝 Thanks to

- [quantumfate](https://github.com/quantumfate)

&nbsp;

<p align="center">
 <img src="https://raw.githubusercontent.com/catppuccin/catppuccin/main/assets/footers/gray0_ctp_on_line.svg?sanitize=true" />
</p>

<p align="center">
 Copyright &copy; 2021-present <a href="https://github.com/catppuccin" target="_blank">Catppuccin Org</a>
</p>

<p align="center">
 <a href="https://github.com/catppuccin/catppuccin/blob/main/LICENSE"><img src="https://img.shields.io/static/v1.svg?style=for-the-badge&label=License&message=MIT&logoColor=d9e0ee&colorA=363a4f&colorB=b7bdf8"/></a>
</p>
