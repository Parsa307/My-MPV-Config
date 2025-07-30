# My MPV Config

This is my custom configuration for [mpv](https://mpv.io/), a powerful and customizable media player. It's optimized for a smooth playback, and a good default experience. Suitable for anime watching. Tested on Arch Linux.

You may want to tweak some options depending on your system, display, or personal preferences.

## 📋 Sources & Inspiration

Configuration based on these excellent guides and setups:

- [Video Playback Guide by iamscum (WordPress)](https://iamscum.wordpress.com/guides/videoplayback-guide/)
- [MPV Manual](https://mpv.io/manual/stable/)
- [mpv.conf Guide by mpv-player (GitHub)](https://raw.githubusercontent.com/mpv-player/mpv/release/0.40/etc/mpv.conf)
- [mpv.conf Guide by iamscum (WordPress)](https://iamscum.wordpress.com/guides/videoplayback-guide/mpv-conf/)
- [mpv.conf on GitLab (iamscum)](https://gitlab.com/iamscum_website/config_mpv/-/blob/main/mpv.conf)
- [input.conf on GitLab (iamscum)](https://gitlab.com/iamscum_website/config_mpv/-/blob/main/input.conf)
- [thumbfast.conf on GitHub (po5)](https://raw.githubusercontent.com/po5/thumbfast/master/thumbfast.conf)
- [sub-select Wiki on GitHub (CogentRedTester)](https://github.com/CogentRedTester/mpv-sub-select/wiki/Example-Configs)

## ✅ Features

- Keep Open is enabled.
- Default OSC is disabled. Use [`ModernZ`](https://github.com/Samillion/ModernZ)
- High-quality video rendering with `gpu-next` and Vulkan
- Hardware decoding enabled
- HDR enabled
- Automatic language and subtitle preferences (Japanese audio, English subs)
- High-quality screenshots saved to `~/Pictures/Screenshots` (Linux) or `%USERPROFILE%\Pictures\Screenshots` (Windows)
- Subtitle timing fixes and fallback settings
- Custom key bindings for volume, frame-step, fullscreen toggle, mute, and more
- Compatible with [`sub-select`](https://github.com/CogentRedTester/mpv-sub-select) for better subtitle stream handling

## 💡 Notes

- You may want to adjust `alang`, `slang`, and interpolation settings to your own preferences.
- Caps Lock can interfere with key bindings that differentiate between lowercase and uppercase (e.g., `m` vs `M`).
- This setup avoids unnecessary complexity. but you can explore features like debanding, shaders if you want more.
- `sub-select` is recommended to auto-pick the best subtitle track. It's especially helpful when dealing with multiple sub streams like signs & songs vs full subs.

## 🔧 Where to Put These

Place the following files in your mpv config folder:

- `mpv.conf` → `~/.config/mpv` (Linux) or `%APPDATA%\mpv` (Windows)
- `input.conf` → same location as above
- `thumbfast.conf` → `~/.config/mpv/script-opts` (Linux) or `%APPDATA%\mpv\script-opts` (Windows)
- `sub-select.json` → `~/.config/mpv/script-opts` (Linux) or `%APPDATA%\mpv\script-opts` (Windows)
