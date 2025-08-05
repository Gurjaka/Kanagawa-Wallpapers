
---

<div align="center">

<img alt="Nix-Snowflake" src="./kanagawa.svg" width="180px"/>

# <samp>Kanagawa Wallpapers</samp>

![GitHub Repo stars](https://img.shields.io/github/stars/Gurjaka/Kanagawa-Wallpapers?style=for-the-badge&labelColor=1f1f28&color=ff7a93) ![GitHub last commit](https://img.shields.io/github/last-commit/Gurjaka/Kanagawa-Wallpapers?style=for-the-badge&labelColor=1f1f28&color=ff7a93) ![GitHub repo size](https://img.shields.io/github/repo-size/Gurjaka/Kanagawa-Wallpapers?style=for-the-badge&labelColor=1f1f28&color=ff7a93)

### A tranquil collection of wallpapers inspired by the elegant Kanagawa color palette, designed to bring a calm and balanced atmosphere to your desktop with minimalist and refined visuals. 🌊🎨

</div>

## Why You’ll Love It ✨

* **High-Quality Resolution**: Crisp and sharp wallpapers optimized for any screen size. 📸
* **Kanagawa Inspired**: A soothing and balanced color scheme that enhances focus and calmness. 🎨
* **Wide Compatibility**: Works flawlessly across all major desktop environments and window managers. 🖥️
* **Easy to Use**: Simple to set up and integrate into your workflow or system configuration. ⚙️

## Installation 🛠️

Add Kanagawa Wallpapers to your setup in just a few steps:

1. **Clone the repository**:

```bash
git clone https://github.com/Gurjaka/Kanagawa-Wallpapers.git
```

### OR

2. **Use [nix flakes](https://wiki.nixos.org/wiki/Flakes)**:

2.1 Add the following input to your `flake.nix`:

```nix
inputs = {
  kanagawa-wallpapers.url = "github:Gurjaka/Kanagawa-Wallpapers";
  ...
}
```

2.2 Link the wallpapers to your preferred folder with Home Manager:

```nix
{
  inputs, 
  pkgs, 
  ...
}: {
  home.file = {
    "path/to/dir" = {
      source = inputs.kanagawa-wallpapers.packages."${pkgs.system}".default;
      recursive = true;
    };
  };
}
```

Then just browse the wallpapers folder and pick the one that suits your mood. 📂

## Setting It Up 🔧

Set these wallpapers on any desktop environment with ease.

If you use Linux and `feh`, set your wallpaper by running:

```bash
feh --bg-scale /path/to/wallpaper.jpg
```

## Contributing 🤝

Got a wallpaper idea or improvements? Fork the repo, add your work, and open a pull request. I’ll review and merge it! 💻

## License 📜

This project is available under the [MIT License](LICENSE). 🖤

---
