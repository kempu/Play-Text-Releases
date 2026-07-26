# Play Text — downloads

Binary distribution for **Play Text** (macOS + iOS reader with word highlighting).
This repository holds no source code — only released artifacts:

- `PlayText-<version>.zip` — the macOS app, fetched by its built-in updater.
- The **on-device voice models**, downloaded on demand from the app's Settings when
  you enable the voice that needs them. None of them ship inside the app; each lives
  under its own release tag:

  | Voice | Tag | Assets |
  | --- | --- | --- |
  | Kokoro-82M | `kokoro-v1.0` | `kokoro-v1_0.safetensors`, `voices.npz` |
  | KittenTTS | `kittentts-v0.8` | `kitten-tts.onnx`, `kitten-voices.npz`, `kitten-config.json`, `kitten-manifest.json` |
  | Inflect-Micro-v2 | `inflect-micro-v2` | `inflect-duration.onnx`, `inflect-decode.onnx`, `inflect-manifest.json` |

  The app verifies each download before installing it, so please don't replace an
  asset in place — publish a new tag instead.

See [Releases](../../releases).
