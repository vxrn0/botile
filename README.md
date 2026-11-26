![Botile](.github/preview.webp)

# Botile

[![Built with OpenCode](https://opencode.ai/brand/badges/opencode-built-with-f-light-20.svg)](https://opencode.ai) [![Version](https://img.shields.io/github/v/release/vxrn0/botile?style=flat-square&label=Version&labelColor=4B4B4B&color=1F1F1F)](https://github.com/vxrn0/botile/releases/latest)

[Русская версия](ru/README.ru.md)

Botile gives Telegram bot avatars a rounded-square shape with a customizable
outline. Other avatars keep the shape chosen by the client.

The shape is there for one practical reason: bots are easy to tell apart from
people and channels at a glance, in a chat list or in a group where everyone
writes at once.

## Features

- Rounded-square bot avatars.
- Theme-aware outline palette: Theme, Accent, White, Black.
- Adjustable outline thickness.
- Settings labels follow the client language: Russian or English, with English
  fallback.

## Compatibility

- exteraless `>= 12.10.6` — the only supported and tested client
- exteraGram — does not work (unsupported)
- AyuGram — same plugin API, but not tested; treat as unverified
- Plugin SDK `>= 1.4.5.3`
- Version `1.0.1`

## Install

1. Settings → Plugins: enable the plugin engine and developer mode.
2. Import `plugin/botile.plugin` (or just open the file from a chat).
3. Confirm the requested `hooks` permission.

## Updates

New releases are posted in [@vxrn0](https://t.me/vxrn0).

## License

MIT — see [LICENSE](LICENSE.md).
