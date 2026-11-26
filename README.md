![Botile](.github/preview.webp)

# Botile

[![Built with OpenCode](https://opencode.ai/brand/badges/opencode-built-with-f-light-20.svg)](https://opencode.ai) [![Version](https://img.shields.io/github/v/release/vxrn0/botile?style=flat-square&label=Version&labelColor=4B4B4B&color=1F1F1F)](https://github.com/vxrn0/botile/releases/latest) [![Built for exteraGram](https://img.shields.io/badge/Built%20for-exteraGram-F54142.svg?style=flat-square&labelColor=1F1F1F&logo=data%3Aimage%2Fsvg%2Bxml%3Bbase64%2CPHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAxOTIgMTkyIiBmaWxsPSJub25lIj48cGF0aCBzdHJva2U9IiNGNTQxNDIiIHN0cm9rZS13aWR0aD0iMTIiIGQ9Ik0xNDQuODkgMzEuMjEyYzEyLjU3My00LjEwNyAyMC4wMjUgMi41NTMgMTYuMDI2IDE1LjA0NC0xMC4wMzggMzEuMzkxLTI5Ljc0OSA4OC42NTMtNDIuMjc3IDEyNC44MS0zLjI4MSA5LjQ1Ny0xOC40NjMgOS4wODctMjIuMjc1LS4xNzEtNi41NC0xNS44NzMtMTYuMTY4LTM0LjM1MS0yOS4zMDgtNDcuODE5LTEyLjU2NS0xMi44NzYtMzAuMTYtMjIuMTg1LTQ1Ljc4My0yOC41NS05LjUxNS0zLjg3Ny05Ljg1Mi0xOS43MDYtLjA3NS0yMi44OTVMMTQ0Ljg5IDMxLjIxWiIvPjwvc3ZnPg%3D%3D)](https://exteragram.app)

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

- exteraless `>= 12.10.6` — the only client where Botile was tested
- exteraGram and AyuGram share the same plugin API but were not tested; treat
  them as unverified
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
