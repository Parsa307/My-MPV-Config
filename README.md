# My MPV Config

This is my custom configuration for [mpv](https://mpv.io/), a powerful and customizable media player. It's optimized for a smooth playback, and a good default experience. Suitable for anime watching. Tested on Arch Linux.

⚠️ Windows Users, we strongly advise you to do not use MPV. It has weird issues for Windows. If you're running to freezing issues, Please don't open a GitHub Issue. You could try undoing this [commit](https://github.com/Parsa307/My-MPV-Config/commit/1302797647384ee899a4a5f72a33fd7305ac8beb) Downside it uses More Memory.

You may want to tweak some options depending on your system, display, or personal preferences.

## 📋 Sources & Inspiration

Configuration based on these excellent guides and setups:

- [MPV Manual](https://mpv.io/manual/stable/)
- [mpv.conf Guide by mpv-player (GitHub)](https://raw.githubusercontent.com/mpv-player/mpv/release/0.40/etc/mpv.conf)
- [thumbfast.conf on GitHub (po5)](https://raw.githubusercontent.com/po5/thumbfast/master/thumbfast.conf)
- [sub-select Wiki on GitHub (CogentRedTester)](https://github.com/CogentRedTester/mpv-sub-select/wiki/Example-Configs)

## ✅ Features

- Keep open enabled
- Default OSC disabled. Use [`ModernZ`](https://github.com/Samillion/ModernZ) (More modern)
- High-quality video rendering with `gpu-next` and Vulkan
- Hardware decoding enabled
- HDR enabled
- Automatic language and subtitle preferences (Japanese audio, English subs) (If Japanese Audio doesn't exist, it falls back to English and uses no subs)
- WEBP loseless quality screenshots saved to `~/Pictures/Screenshots` (Linux) or `%USERPROFILE%\Pictures\Screenshots` (Windows)
- Subtitle fix timing enabled
- Custom key bindings for volume, frame-step
- Hardware decoding enabled for thumbfast
- Compatible with [`sub-select`](https://github.com/CogentRedTester/mpv-sub-select) for better subtitle stream handling

## 💡 Notes

- You may want to adjust `alang`, `slang` to your own preferences.
- `sub-select` is recommended to auto-pick the best subtitle track. It's especially helpful when dealing with multiple sub streams like signs & songs vs full subs.

## 🔧 Where to Put These

Place the following files in your mpv config folder:

- `mpv/mpv.conf` (Linux) or `mpv\mpv.conf` (Windows) → `~/.config/mpv` (Linux) or `%APPDATA%\mpv` (Windows)
- `mpv/input.conf` (Linux) or `mpv\input.conf` (Windows) → `~/.config/mpv` (Linux) or `%APPDATA%\mpv` (Windows)
- `mpv/script-opts/thumbfast.conf` (Linux) or `mpv\script-opts\thumbfast.conf` (Windows) → `~/.config/mpv/script-opts` (Linux) or `%APPDATA%\mpv\script-opts` (Windows)
- `mpv/script-opts/sub-select.json` (Linux) or `mpv\script-opts\sub-select.json` (Windows) → `~/.config/mpv/script-opts` (Linux) or `%APPDATA%\mpv\script-opts` (Windows)

## My Specs
- Host: MSI Raider GE76 12UGS
- CPU: 12th Gen Intel(R) Core(TM) i7-12700H (20) @ 4.70 GHz
- GPU: NVIDIA Geforce RTX 3070 Ti Laptop GPU
- Memory: 31.10 GiB
