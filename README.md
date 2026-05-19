# My MPV Config

[![Please don't upload to GitHub](https://nogithub.codeberg.page/badge-sq.svg)](https://nogithub.codeberg.page)

This is my custom configuration for [mpv](https://mpv.io), a powerful and customizable media player. It's optimized for a smooth playback, and a good default experience. Suitable for **Anime** watching.

You may want to tweak some options depending on your system, display, or personal preferences.

If you're experiencing issues, try Troubleshooting.

# 📋 Sources

Configuration based on these excellent guides and setups:

- [MPV Manual](https://mpv.io/manual/stable)
- [mpv.conf Guide by mpv-player (GitHub)](https://github.com/mpv-player/mpv/blob/v0.40.0/etc/mpv.conf)
- [thumbfast.conf on GitHub (po5)](https://github.com/po5/thumbfast/blob/master/thumbfast.conf)
- [sub-select Wiki on GitHub (CogentRedTester)](https://github.com/CogentRedTester/mpv-sub-select/wiki/Example-Configs)

# ✅ Features

- Ignore hidden is disabled for autoload.
- Default OSC disabled, use [ModernZ](https://github.com/Samillion/ModernZ) (More modern).
- High-quality video rendering with gpu-next and Vulkan.
- Hardware decoding enabled.
- HDR enabled.
- Automatic language and subtitle preferences (Japanese audio, English subs).
- PNG screenshots saved to `~/Pictures/Screenshots` (Linux) or `%USERPROFILE%\Pictures\Screenshots` (Windows).
- Subtitle with matching audio disabled.
- Subtitle fix timing enabled.
- Custom key bindings for volume, frame-step.
- Hardware decoding enabled for thumbfast.
- Compatible with [sub-select](https://github.com/CogentRedTester/mpv-sub-select) for better subtitle stream handling.

# 💡 Notes

- You may want to adjust alang, slang to your own preferences.
- I also use [autoload](https://raw.githubusercontent.com/mpv-player/mpv/master/TOOLS/lua/autoload.lua) is recommended to auto-add media files to the MPV playlists.
- sub-select is recommended to auto-pick the best subtitle track. It's especially helpful when dealing with multiple sub streams like signs & songs vs full subs.

# 🔧 Where to Put These

Place the following files in your mpv config folder:

- `mpv.conf` (Linux) or `mpv\mpv.conf` (Windows) → `~/.config/mpv` (Linux) or `%APPDATA%\mpv` (Windows)
- `input.conf` (Linux) or `mpv\input.conf` (Windows) → `~/.config/mpv` (Linux) or `%APPDATA%\mpv` (Windows)
- `script-opts/thumbfast.conf` (Linux) or `script-opts\thumbfast.conf` (Windows) → `~/.config/mpv` (Linux) or `%APPDATA%\mpv` (Windows)
- `script-opts/sub-select.json` (Linux) or `script-opts\sub-select.json` (Windows) → `~/.config/mpv` (Linux) or `%APPDATA%\mpv` (Windows)
- `script-opts/autoload.conf` (Linux) or `script-opts\autoload.conf` (Windows) → `~/.config/mpv` (Linux) or `%APPDATA%\mpv` (Windows)

# ⚙️ Troubleshooting
- Enable caching by undoing this [commit](../../../commit/1302797647384ee899a4a5f72a33fd7305ac8beb), [GitHub commit](https://github.com/Parsa307/My-MPV-Config/commit/1302797647384ee899a4a5f72a33fd7305ac8beb). (Helps freezing issues on NTFS). (Downside, uses More System Memory)
- Changing the filesystem. (I recommend EXT4 or BTRFS)
