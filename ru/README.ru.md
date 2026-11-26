![Botile](../.github/preview.webp)

# Botile

[![Built with OpenCode](https://opencode.ai/brand/badges/opencode-built-with-f-light-20.svg)](https://opencode.ai) [![Version](https://img.shields.io/github/v/release/vxrn0/botile?style=flat-square&label=Version&labelColor=4B4B4B&color=1F1F1F)](https://github.com/vxrn0/botile/releases/latest) [![Built for exteraGram](https://img.shields.io/badge/Built%20for-exteraGram-F54142.svg?style=flat-square&labelColor=1F1F1F&logo=data%3Aimage%2Fsvg%2Bxml%3Bbase64%2CPHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAxOTIgMTkyIiBmaWxsPSJub25lIj48cGF0aCBzdHJva2U9IiNGNTQxNDIiIHN0cm9rZS13aWR0aD0iMTIiIGQ9Ik0xNDQuODkgMzEuMjEyYzEyLjU3My00LjEwNyAyMC4wMjUgMi41NTMgMTYuMDI2IDE1LjA0NC0xMC4wMzggMzEuMzkxLTI5Ljc0OSA4OC42NTMtNDIuMjc3IDEyNC44MS0zLjI4MSA5LjQ1Ny0xOC40NjMgOS4wODctMjIuMjc1LS4xNzEtNi41NC0xNS44NzMtMTYuMTY4LTM0LjM1MS0yOS4zMDgtNDcuODE5LTEyLjU2NS0xMi44NzYtMzAuMTYtMjIuMTg1LTQ1Ljc4My0yOC41NS05LjUxNS0zLjg3Ny05Ljg1Mi0xOS43MDYtLjA3NS0yMi44OTVMMTQ0Ljg5IDMxLjIxWiIvPjwvc3ZnPg%3D%3D)](https://exteragram.app)

[English version](../README.md)

Botile придаёт аватарам Telegram-ботов скруглённую квадратную форму с
настраиваемой обводкой. Остальные аватары сохраняют форму, выбранную клиентом.

Форма нужна для одной практической вещи: ботов легко отличить от людей и каналов
с первого взгляда — в списке чатов или в группе, где все пишут одновременно.

## Возможности

- Скруглённые квадратные аватары ботов.
- Адаптивная к теме палитра обводки: «Тема», «Акцент», «Белая», «Чёрная».
- Настраиваемая толщина обводки.
- Подписи настроек следуют языку клиента: русский или английский, с fallback
  на английский.

## Совместимость

- exteraless `>= 12.10.6` — единственный клиент, в котором Botile проверялся
- exteraGram и AyuGram используют тот же API плагинов, но не тестировались;
  считайте их поддержку непроверенной
- SDK плагинов `>= 1.4.5.3`
- Версия `1.0.1`

## Установка

1. Настройки → Plugins: включить движок плагинов и режим разработчика.
2. Импортировать `plugin/botile.plugin` (или просто открыть файл из чата).
3. Подтвердить разрешение `hooks`.

## Обновления

Новые версии публикуются в [@vxrn0](https://t.me/vxrn0).

## Лицензия

MIT — см. [LICENSE.ru.md](LICENSE.ru.md).
