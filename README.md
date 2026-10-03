# browser-use-agent

Tarayıcı kullanan bir ajan için Python iskeleti. Paket `browser-use` kütüphanesine bağlı. Şu anki giriş noktası bir karşılama satırı basar; ajan akışı bu fonksiyonun içine yazılır.

## Kurulum

Python 3.12 ve [uv](https://docs.astral.sh/uv/) gerekir.

```bash
cd browser-use-agent
uv sync
uv run browser-use-agent
```

## Nasıl kuruldu

Proje tanımı `pyproject.toml` içinde. Derleme sistemi `uv_build`. Bağımlılık `browser-use`. Komut adı `browser-use-agent`, fonksiyon `browser_use_agent:main`. Sanal ortam `.venv` klasöründedir ve depoya girmez.

Kütüphane, bir dil modeline tarayıcıda tıklama, yazma ve sayfa okuma adımları verdirmek için kullanılır. Bu depodaki `main` henüz o döngüyü başlatmıyor.
