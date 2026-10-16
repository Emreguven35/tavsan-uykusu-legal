# Tavşan Uykusu — Yasal Metinler

Tavşan Uykusu mobil uygulamasının yasal metinlerinin yayın deposu.
GitHub Pages üzerinden sunulur.

- Gizlilik Politikası ve Aydınlatma Metni: https://emreguven35.github.io/tavsan-uykusu-legal/gizlilik.html
- Kullanım Koşulları: https://emreguven35.github.io/tavsan-uykusu-legal/kosullar.html
- Açık Rıza Metni (bebeğe ait uyku ve gelişim bilgileri): https://emreguven35.github.io/tavsan-uykusu-legal/acik-riza.html
- Açık Rıza Metni (Anne Sesi): https://emreguven35.github.io/tavsan-uykusu-legal/anne-sesi-riza.html
- Destek ve sık sorulanlar: https://emreguven35.github.io/tavsan-uykusu-legal/destek.html
- Hesap silme (Google Play şartı): https://emreguven35.github.io/tavsan-uykusu-legal/hesap-silme.html
- Şifre sıfırlama: https://emreguven35.github.io/tavsan-uykusu-legal/sifre-sifirla.html

Destek, hesap silme ve şifre sıfırlama sayfaları elle yazılmıştır (markdown'dan
üretilmez). Kaynakları mobil depoda `mobile/legal/site/` altında sürüm
takibindedir; index.html'deki bağlantıları da üretici betik ekler.

## Nasıl güncellenir

Bu depodaki HTML dosyaları **burada elle düzenlenmez**.
Kaynak, mobil uygulama deposundaki markdown dosyalarıdır:

    mobile/legal/gizlilik.md
    mobile/legal/kosullar.md
    mobile/legal/acik-riza.md
    mobile/legal/anne-sesi-riza.md

Metni orada düzenleyin, sonra:

    node scripts/build-legal-site.mjs

komutuyla `mobile/legal/site/` altındaki HTML'i yeniden üretip buraya kopyalayın.

**Kopyalarken bu klasörü silmeyin.** `mobile/legal/site/` içindeki dosyaları
üzerine yazarak kopyalayın; klasörü boşaltıp yeniden doldurmayın. `.nojekyll`,
README.md ve `.git` yalnız bu depoda vardır, silinirse GitHub Pages yayını bozulur.

Sayfalar tek dosyalık statik HTML'dir: CSS gömülüdür, hiçbir dış bağımlılık
(font, CDN, script, analitik) yoktur.

Veri sorumlusu: İlayda Kani (Tavşan Uykusu) · tavsanuykusu@hotmail.com
