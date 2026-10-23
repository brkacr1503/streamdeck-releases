# streamdeck — kurulum ve güncellemeler

Bu depo yalnızca **streamdeck** eşlik uygulamasının (ESP32-S3 dokunmatik Stream Deck için Windows uygulaması) imzalı kurulum paketlerini ve güncelleme bilgisini taşır. Kaynak kod burada değildir.

## Kurulum

1. `latest.json` dosyasındaki sürümün klasörünü açın (ör. `v0.6.1/`).
2. `streamdeck_<sürüm>_x64-setup.exe` dosyasını indirip çalıştırın. Kurulum yönetici izni istemez.
3. Paket kod imzalı olmadığı için Windows SmartScreen uyarabilir: "Ek bilgi" → "Yine de çalıştır".

Kurulduktan sonra uygulama yeni sürümleri kendisi bulur ve sorar; kartın firmware'i de uygulamanın içinden güncellenir.

## Dosyalar

| Dosya | Ne |
|---|---|
| `latest.json` | Son sürüm, notları, imzası ve indirme adresi (Tauri updater bunu okur) |
| `v<sürüm>/streamdeck_<sürüm>_x64-setup.exe` | Kurulum paketi |
| `v<sürüm>/streamdeck_<sürüm>_x64-setup.exe.sig` | Güncelleme imzası: uygulama yalnızca bu imzası doğrulanan paketi kurar |

Dosyaları yayın hattı yükler; elle değiştirilmez.
