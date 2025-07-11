# My MPV Config

This is my custom configuration for [mpv](https://mpv.io/), a powerful media player. It's optimized for a clean look, smooth playback, and a good default experience.

You may want to tweak some options depending on your system, display, or preferences.

---

## 📋 Sources & Inspiration

Configuration based on these excellent guides and setups:

- [Video Playback Guide by iamscum (WordPress)](https://iamscum.wordpress.com/guides/videoplayback-guide/)
- [mpv.conf Guide by iamscum (WordPress)](https://iamscum.wordpress.com/guides/videoplayback-guide/mpv-conf/)
- [mpv.conf on GitLab (iamscum)](https://gitlab.com/iamscum_website/config_mpv/-/blob/main/mpv.conf)
- [input.conf on GitLab (iamscum)](https://gitlab.com/iamscum_website/config_mpv/-/blob/main/input.conf)

---

## ✅ Features

- High-quality video rendering with `gpu-next` and Vulkan
- Hardware decoding enabled
- Auto-language/subtitle preference (Japanese audio, English subs)
- High-quality screenshots saved to `~/Pictures/Screenshots`
- Subtitle timing fixes and fallback settings
- Interpolation enabled for smoother playback
- Customized key bindings (volume, frame-step, fullscreen, mute, etc.)

---

## 💡 Notes

- You may want to adjust `alang`, `slang`, and interpolation settings to your own preferences.
- Caps Lock can interfere with key bindings that differentiate between lowercase and uppercase (e.g., `m` vs `M`).
- This setup avoids unnecessary complexity — but you can explore features like debanding, shaders if you want more.

---

## 🔧 Where to Put These

Place the following files in your mpv config folder:

- `mpv.conf` → `~/.config/mpv` (Linux) or `%APPDATA%\mpv` (Windows)
- `input.conf` → same location as above
