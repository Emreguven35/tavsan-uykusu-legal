# Tavşan Uykusu — Yasal Metinler

Tavşan Uykusu mobil uygulamasının yasal metinlerinin yayın deposu.
GitHub Pages üzerinden sunulur.

- Gizlilik Politikası ve Aydınlatma Metni: https://emreguven35.github.io/tavsan-uykusu-legal/gizlilik.html
- Kullanım Koşulları: https://emreguven35.github.io/tavsan-uykusu-legal/kosullar.html
- Açık Rıza Metni (bebeğe ait uyku ve gelişim bilgileri): https://emreguven35.github.io/tavsan-uykusu-legal/acik-riza.html
- Açık Rıza Metni (Anne Sesi): https://emreguven35.github.io/tavsan-uykusu-legal/anne-sesi-riza.html
- Destek ve sık sorulanlar: https://emreguven35.github.io/tavsan-uykusu-legal/destek.html
  (elle yazılmış sayfa — markdown'dan ÜRETİLMEZ; site yeniden üretilip kopyalanırken
  destek.html korunmalı ve index.html'deki Destek bağlantısı yeniden eklenmeli)

## Nasıl güncellenir

Bu depodaki HTML dosyaları **elle düzenlenmez** — üretilmiş çıktıdır.
Kaynak, mobil uygulama deposundaki markdown dosyalarıdır:

    mobile/legal/gizlilik.md
    mobile/legal/kosullar.md
    mobile/legal/acik-riza.md
    mobile/legal/anne-sesi-riza.md

Metni orada düzenleyin, sonra:

    node scripts/build-legal-site.mjs

komutuyla `mobile/legal/site/` altındaki HTML'i yeniden üretip buraya kopyalayın.

Sayfalar tek dosyalık statik HTML'dir: CSS gömülüdür, hiçbir dış bağımlılık
(font, CDN, script, analitik) yoktur.

Veri sorumlusu: İlayda Kani (Tavşan Uykusu) · tavsanuykusu@hotmail.com
