# browser-use-agent

Tarayıcı kullanan bir ajan için Python iskeleti. Paket `browser-use` kütüphanesine bağlı. Şu anki giriş noktası bir karşılama satırı basar; ajan akışı bu fonksiyonun içine yazılır.

A Python skeleton for an agent that uses a browser. The package depends on the `browser-use` library. The current entry point prints a greeting; the agent loop belongs inside that function.

## Kurulum / Setup

Python 3.12 ve [uv](https://docs.astral.sh/uv/) gerekir. / Requires Python 3.12 and [uv](https://docs.astral.sh/uv/).

```bash
cd browser-use-agent
uv sync
uv run browser-use-agent
```

## Teknoloji / Stack

Proje tanımı `pyproject.toml` içinde. Derleme sistemi `uv_build`. Bağımlılık `browser-use`. Komut adı `browser-use-agent`, fonksiyon `browser_use_agent:main`. Sanal ortam `.venv` klasöründedir ve depoya girmez. Kütüphane, bir dil modeline tarayıcıda tıklama, yazma ve sayfa okuma adımları verdirmek için kullanılır. Bu depodaki `main` o döngüyü henüz başlatmıyor.

The project is defined in `pyproject.toml`. The build system is `uv_build`. The dependency is `browser-use`. The command is `browser-use-agent` and the function is `browser_use_agent:main`. The virtualenv is `.venv` and stays out of the repo. The library lets a language model click, type, and read pages. `main` in this repo does not start that loop yet.
