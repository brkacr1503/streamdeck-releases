# streamdeck

Dokunmatik ekranlı **streamdeck** kartının Windows uygulaması. Kartın sayfalarını ve butonlarını buradan düzenlersiniz. Uygulama Spotify'da çalan şarkıyı karta gönderir, kartın yazılımını da günceller.

## İndir

### [⬇ streamdeck-setup.exe (son sürüm)](https://github.com/brkacr1503/streamdeck-releases/releases/latest/download/streamdeck-setup.exe)

Windows 10 ve 11 (64 bit) için. Önceki sürümler ve neler değiştiği: [Sürümler](https://github.com/brkacr1503/streamdeck-releases/releases)

## Kurulum

1. Yukarıdaki bağlantıdan `streamdeck-setup.exe` dosyasını indirin.
2. Tarayıcı dosyayı "yaygın olarak indirilmiyor" diye bekletebilir. İndirilenler listesinde dosyanın yanındaki menüden **Sakla** (Edge'de **Yine de sakla**) seçin.
3. Dosyayı çalıştırın. Mavi bir **"Windows bilgisayarınızı korudu"** penceresi çıkarsa **Ek bilgi**'ye, sonra **Yine de çalıştır**'a tıklayın.
4. Kurulum birkaç saniye sürer ve yönetici izni istemez. Uygulama saatin yanındaki simge tepsisinde durur. Windows açılınca kendiliğinden başlaması için: **Ayarlar → Windows açılışında başlat**.

### Neden uyarı çıkıyor?

Bu uyarılar dosyada virüs olduğu anlamına gelmez. Windows'un yayımcıyı tanıması için yıllık ücretli bir kod imzalama sertifikası gerekiyor. Bu uygulamada böyle bir sertifika yok. Bu yüzden Windows ve tarayıcılar, az indirilen her imzasız dosyada yaptıkları gibi uyarıyor.

- Kurulum paketini bu deponun yayın hattı derleyip yükler; dosyalar elle değiştirilmez.
- Uygulama internete yalnızca bu depodan yeni sürüm olup olmadığına bakmak ve güncellemeyi indirmek için çıkar.
- Güncellemeler imzalıdır: uygulama, imzası tutmayan bir paketi kurmaz.

## Kartı bağlamak

**Kabloyla:** Kartı, üzerinde **USB** yazan girişinden bilgisayara takın. Uygulama kartı kendisi bulur ve sol üstte **Bağlı** yazar.

**Bluetooth'la (kablosuz):**

1. Kartta **Ayarlar → BLE eşleştir**'e dokunun. Uygulamada **Kart → Bluetooth → Eşleştirme kipini aç** da aynı işi yapar.
2. Windows'ta **Ayarlar → Bluetooth ve cihazlar → Cihaz ekle → Bluetooth** deyin ve listeden **streamdeck**'i seçin.
3. Bir kez eşleştirmek yeter. Kart bilgisayara takılı değilken, örneğin şarj aletindeyken, tuşlar Bluetooth'tan gider ve uygulama karta Bluetooth'tan bağlanır. Kablo takılınca ikisi de kendiliğinden USB'ye döner.

## Güncellemeler

- Yeni sürüm çıkınca uygulama üstte haber verir; **Kur ve yeniden başlat** demeniz yeter.
- Elle bakmak için: **Ayarlar → Güncellemeleri denetle**.
- Kartın yazılımı uygulamanın içinde gelir. **Kart** sekmesinde "Yeni firmware var" yazarsa **Güncelle**'ye basın. Kabloyla ~20 sn, Bluetooth'la ~40 sn sürer. Yarıda kalırsa kart eski yazılımla açılır; yeniden deneyebilirsiniz.

## Kaldırmak

**Windows Ayarlar → Uygulamalar → Yüklü uygulamalar → streamdeck → Kaldır**

---

<details>
<summary>Bu depoda neler var</summary>

Bu depo yalnızca kurulum paketlerini ve güncelleme bilgisini taşır; kaynak kod burada değildir. Dosyaları yayın hattı yükler.

| Dosya | Ne |
|---|---|
| [Sürümler](https://github.com/brkacr1503/streamdeck-releases/releases) | Her sürümün notu ve `streamdeck-setup.exe` kurulum paketi |
| `latest.json` | Son sürüm, notu, imzası ve indirme adresi; uygulama güncellemeyi buradan bulur |
| `v<sürüm>/streamdeck_<sürüm>_x64-setup.exe` | Uygulamanın güncellerken indirdiği kurulum paketi (Sürümler'dekiyle aynı dosya) |
| `v<sürüm>/streamdeck_<sürüm>_x64-setup.exe.sig` | Güncelleme imzası: uygulama yalnızca bu imzası doğrulanan paketi kurar |

</details>
