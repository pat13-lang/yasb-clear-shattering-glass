# 💎 bliqx's clear shattering glass - YASB Theme

A premium, glassmorphic status bar configuration for **YASB (Yet Another Status Bar)**. This theme creates an elegant, semi-transparent "shattering glass" aesthetic by utilizing subtle alpha channels (`rgba`), system blurs, and stylized popups.

---

## 🎨 Theme Overview & Typography

The status bar initializes a `100%` width, top-aligned canvas (`height: 30px`) under a clean transparent setup. The text engine is balanced across specific default typefaces:

*   **Primary Text & Data**: `"Segoe UI"`, `"JetBrainsMono NFP"` (`font-weight: 600`)
*   **System UI & Elements**: `"JetBrainsMono NFP"`
*   **System Indicators**: `"Segoe Fluent Icons"`

<img width="959" height="599" alt="preview" src="https://github.com/user-attachments/assets/50fc585a-f142-4d4f-8db6-fec2a6f93262" />

### 🎛️ Widget Layout Arrangement
*   **Left Section**: `home` (Navigation Panel), `taskbar`
*   **Center Section**: `clock` (Formatted system time & Calendar)
*   **Right Section**: `systray`, `cpu`, `volume`, `notifications`, `power_menu`, `weather`

---

## 🚀 Getting Started

### 📋 Prerequisites
*   **YASB** successfully installed on your machine.
*   **Fonts Installed**: Make sure `"Segoe UI"`, `"Segoe Fluent Icons"`, and a complete variant of `"JetBrainsMono Nerd Font"` are installed for glyph layouts (`\ue62a`, `\uf4bc`, etc.) to show up properly.
*   **Weather Access**: A free API key from [WeatherAPI.com](https://weatherapi.com).

### 🔧 Installation Steps

1.  Navigate to your local YASB folder inside your profile root directory:
    ```cmd
    cd %USERPROFILE%/.config/yasb/
    ```
2.  Drop your `config.yaml` and `styles.css` files directly into this directory.
3.  Open `config.yaml` and paste your unique authorization token inside the weather category:
    ```yaml
    api_key: "YOUR_WEATHERAPI_KEY_HERE"
    ```
4.  Launch or refresh YASB. The settings use `watch_config: true` and `watch_stylesheet: true`, enabling hot-reloading anytime you save text edits.

---

## 🛠️ Color Palette Configuration

The look is built on soft dark glass backgrounds paired with vibrant structural color accents. You can tweak these directly at the top of your `styles.css` file:

| CSS Variable | Description | Value |
| :--- | :--- | :--- |
| `--bg-primary` / `--bg-taskbar` | Semi-transparent main container plates | `rgba(8, 8, 8, 0.4)` |
| `--bg-secondary` | Solid module panels (Tooltips, Launchpad contexts) | `rgba(28, 30, 29, 1)` |
| `--text-primary` | Main text color | `#ffffff` |
| `--text-secondary` | Dimmed/Subtle information text | `rgba(255, 255, 255, 0.54)` |
| `--color-yellow` | Sunny day indicators & Weather forecast graph curves | `#fae93f` |
| `--color-green` | Launchpad selections / Power menu cancel buttons | `#3f925f` |
| `--color-red` | Power menu shutdown triggers / Alerts | `#cb3b42` |
| `--color-light-blue` | Nighttime clear skies color | `rgb(112, 157, 255)` |

---

## 🔍 Widget Specific Styles

*   **Advanced Calendar Engine**: Employs an ultra-bold date label (`89px` tall with a `900` font weight) alongside localized mapping configurations pinned to region code `PL`.
*   **Interactive Weather Card**: Dynamic day components seamlessly track active states with highlighted background borders. Features smooth hourly curves utilizing weather rendering maps.
*   **Power Control Grid**: Features generous layout fields (`240px x 120px` button cards) inside a dark background layout (`--bg-hover-fourth`) with matching green and red confirmation states.
*   **Audio Core Selector**: Dynamic sound containers display standard and active audio hardware lines instantly using clear grey structural borders (`--color-grey`).
*   **System Launchpad Context**: Extends clear background interfaces with precise nested entry formatting (`6px 12px` layout items with custom hover states).

---

## 📄 License

This configuration layout is distributed under the community **MIT License**.
