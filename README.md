# win11-config

> A glass-style Windows 11 setup themed with **Catppuccin Mocha** — clean, minimal, and aesthetic.

Credits for the installation tutorial and Catppuccin config go to [@SleepyCatHey](https://github.com/SleepyCatHey/Ultimate-Win11-Setup).

---

##  What's Included

| Folder/File | Description |
|---|---|
| `windhawk/` | Windhawk mod configs for UI tweaks |
| `flyout/` | Fluent Flyout configuration |
| `cursor/` | Custom cursor theme |
| `wallpapers/` | Wallpapers used in the setup |
| `styles.txt` | Custom styles / CSS overrides |
| `yasb widget.txt` | YASB status bar widget config |
| `Installation.txt` | Step-by-step install guide |

---

##  Installation

### 1. Scoop (Package Manager)

```powershell
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
Invoke-RestMethod -Uri https://get.scoop.sh | Invoke-Expression
```

### 2. Git

```powershell
winget install --id Git.Git -e --source winget
```

### 3. Core Tools

```powershell
# YASB (status bar)
winget install --id AmN.yasb

# Flow Launcher
winget install "Flow Launcher"

# Cava (audio visualizer)
winget install karlstav.cava

# Yazi (terminal file manager) + dependencies
winget install sxyazi.yazi
winget install Gyan.FFmpeg 7zip.7zip jqlang.jq oschwartz10612.Poppler sharkdp.fd BurntSushi.ripgrep.MSVC junegunn.fzf ajeetdsouza.zoxide ImageMagick.ImageMagick

# Set file.exe path for Yazi
setx YAZI_FILE_ONE "C:\Program Files\Git\usr\bin\file.exe"
```

### 4. Shell Extras

```powershell
# PSReadLine (autocomplete)
Install-Module -Name PSReadLine -AllowClobber -Force

# yt-dlp + FFmpeg
winget install yt-dlp
winget install Gyan.FFmpeg

# fzf (fuzzy finder)
winget install -e --id junegunn.fzf

# Fastfetch
scoop install fastfetch
```

### 5. Windhawk (UI Mods)

Download from [windhawk.net](https://windhawk.net/) and apply the configs from the `windhawk/` folder.

### 6. Catppuccin Theme

Follow the full guide by [@SleepyCatHey](https://github.com/SleepyCatHey/Ultimate-Win11-Setup).

### 7. Fluent Flyout

Download from [fluentflyout.com](https://fluentflyout.com/download/) and apply the config from the `flyout/` folder.

---

##  Video Guides

| Topic | Link |
|---|---|
| Terminal + Fastfetch setup | [YouTube](https://www.youtube.com/watch?v=z3NpVq-y6jU) |
| Fluent Flyout | [YouTube](https://www.youtube.com/watch?v=44gS79FdtIg) |
| Cava visualizer | [YouTube](https://www.youtube.com/watch?v=Ehnj5fzWegY) |

---

##  Credits

- Catppuccin config & tutorial — [@SleepyCatHey](https://github.com/SleepyCatHey/Ultimate-Win11-Setup)
- Color palette — [Catppuccin](https://github.com/catppuccin/catppuccin)
