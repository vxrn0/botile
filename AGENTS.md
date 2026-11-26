# AGENTS.md — botile

Single-file plugin for the Telegram client family sharing one Python plugin host:
**exteraGram**, **exteraless**, **AyuGram**. It gives bot avatars a rounded-square
shape with an optional theme-aware frame; other avatars are left alone.

Supported and tested only in exteraless. exteraGram is known not to work
(unsupported); AyuGram is untested (unverified).

The shape exists for distinguishability: a bot should be recognisable as a bot
at a glance, without reading its name, in a chat list or a busy group.

Plugin API (hooks, settings, Chaquopy interop): [`docs/plugin-api.md`](docs/plugin-api.md).
Load the `exteraless-plugin-dev` skill
(`.agents/skills/exteraless-plugin-dev/SKILL.md`) before editing code.

## Layout

| Path | Contents |
|------|----------|
| `plugin/botile.plugin` | The whole plugin: hooks, settings, drawing. Single file by contract. |
| `scripts/package_release.py` | Validates metadata, builds `dist/Botile-<version>.plugin` + `SHA256SUMS`. |
| `tests/test_state_preservation.py` | Host-side mocks for state restore, settings, drawing, reflection. |
| `docs/plugin-api.md` | How plugins for this host family are written. |
| `SECURITY.md` | Supported versions, trusted builds, vulnerability reporting. |
| `.github/` | CI workflow and `preview.webp` for the READMEs. |
| `ru/` | Russian README, license and security policy; English originals stay at the root. |

## Commands

```sh
python3 -m py_compile plugin/botile.plugin
python3 scripts/package_release.py --check
python3 tests/test_state_preservation.py
python3 scripts/package_release.py --output-dir dist
(cd dist && sha256sum -c SHA256SUMS)
```

## Rules

- The `.plugin` file stays at `plugin/botile.plugin`; CI, packaging and tests read
  that exact path.
- Metadata (`__id__`, `__version__`, `__app_version__`, `__sdk_version__`,
  `__permissions__`) must stay literal assignments; `package_release.py` parses
  them with `ast`.
- Hook only the paths listed in the module docstring. Widen a hook only with a
  test proving regular users, groups, channels and custom images are untouched.
- Every applied radius/mark stores its baseline and is restored on clear and
  unload; do not clobber marks set by other code.
- Keep host-side tests runnable without the client or Android: use the mocks,
  they do not replace a device test.
- Name every client you claim support for, and say which ones were never run.
- A change that fits in one commit goes straight to `main`; do not open a PR for it.

## Language

Code, comments, commits and English docs in English. `ru/` is Russian product
documentation; keep it in sync with the English files.
