# Tavşan Uykusu — Yasal Metinler

Tavşan Uykusu mobil uygulamasının yasal metinlerinin yayın deposu.
GitHub Pages üzerinden sunulur.

- Gizlilik Politikası: https://emreguven35.github.io/tavsan-uykusu-legal/gizlilik.html
- Kullanım Koşulları: https://emreguven35.github.io/tavsan-uykusu-legal/kosullar.html

## Nasıl güncellenir

Bu depodaki HTML dosyaları **elle düzenlenmez** — üretilmiş çıktıdır.
Kaynak, mobil uygulama deposundaki markdown dosyalarıdır:

    mobile/legal/gizlilik.md
    mobile/legal/kosullar.md

Metni orada düzenleyin, sonra:

    node scripts/build-legal-site.mjs

komutuyla `mobile/legal/site/` altındaki HTML'i yeniden üretip buraya kopyalayın.

Sayfalar tek dosyalık statik HTML'dir: CSS gömülüdür, hiçbir dış bağımlılık
(font, CDN, script, analitik) yoktur.

Veri sorumlusu: İlayda Kani (Tavşan Uykusu) · mrguven35@gmail.com
