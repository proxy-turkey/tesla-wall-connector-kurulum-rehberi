# ⚡ Tesla Wall Connector Kurulum Rehberi

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Language](https://img.shields.io/badge/dil-T%C3%BCrk%C3%A7e-red.svg)
![Power](https://img.shields.io/badge/g%C3%BC%C3%A7-11kW%20Trifaze-orange)

**Türkiye'de Tesla Wall Connector Gen 3 (Üç Faz / Trifaze 400V, 11 kW) kurulumu için açık kaynaklı, tam kapsamlı rehber.**

Tesla Wall Connector kurmak isteyen ve hangi malzemeleri alması gerektiğini, nasıl kurulacağını arayan kişilere faydalı olması amacıyla hazırlanmıştır.

---

## 🌐 Canlı Demo

**[→ Rehberi tarayıcıda aç](https://proxy-turkey.github.io/tesla-wall-connector-kurulum-rehberi/)**

İnteraktif HTML rehber: malzeme listesi, SVG diyagram, adım adım kurulum, devreye alma ve uyarılar. Harici bağımlılık gerektirmez.

---

## 📁 Dosyalar

| Dosya | Açıklama |
|-------|----------|
| [`tesla-wc-kurulum-rehberi.html`](tesla-wc-kurulum-rehberi.html) | **Ana rehber** — interaktif HTML (SVG diyagram, malzeme tablosu, adım adım kurulum, devreye alma) |
| [`summary.md`](summary.md) | Proje özeti — elektriksel mimari, güç akışı, koruma mimarisi, mühendislik değerlendirmeleri |
| [`malzemeler.csv`](malzemeler.csv) | Tam malzeme listesi — CSV formatında, kategorize edilmiş (20+ kalemler) |

> **Not:** Tesla'nın resmi Wall Connector kurulum kılavuzu için [Tesla'nın destek sayfasını](https://www.tesla.com/support/charging/wall-connector) ziyaret edin.

---

## 🔧 Sistem Mimarisi

Bu rehber, aşağıdaki kurulum mimarisini tarif eder:

```
[Ana Pano: Giriş Barası]
         │
    [QF1: 4P 50A MCB] ── 5m 5×6mm² NYY (Ø25mm Çelik Spiral) ──┐
                                                                ▼
                                                      [Lokal WC Panosu]
                                                    ┌──────────┬─────────┐
                                               [QF2: 40A]  [SPD1: 100kA]  [K1: ENTES]
                                                    │
                                              [FI1: 30mA RCD]
                                                    │
                                              [KM1: 4P Kontaktör]
                                                    │
                                          [Tesla WC Gen 3] → [Araç]
```

### Temel Özellikler

| Özellik | Detay |
|---------|-------|
| **Güç** | 11 kW AC — Üç Faz 400V L-L, faz başına 16A |
| **Topraklama** | Bağımsız lokal TT — Q20 bakır çubuklar + bentonit, <10Ω hedefli |
| **Selektivite** | 50A (ana pano) → 40A (lokal pano) kademeli koruma |
| **Gerilim Koruması** | ENTES GKRC-02F — 207V/253V eşikler, 25s gecikmeli geri dönüş |
| **Parafudr** | Citel DS104RS-230/G/TR 100kA (Tip I+II+III) |
| **Kontaktör** | Siemens 5TT5840-0 (4P 40A, AC-1 sınıfı) |
| **Kaçak Akım** | Siemens 5SV3346-6 (30mA Tip A) + Tesla WC dahili RCD-DD |
| **Kablo** | 5×6mm² NYY — Ø25mm çelik spiral içinde |

---

## ⚠️ Sorumluluk Reddi

> **Bu rehber yalnızca bilgi paylaşımı amacıyla hazırlanmıştır.** Elektrik tesisatı, özellikle de EV şarj sistemleri, **lisanslı bir elektrikçi** tarafından yapılmalıdır. Bu dökümanlardaki bilgiler hiçbir koşulda profesyonel mühendislik danışmanlığının yerine geçmez. Bu projeyi kullanarak oluşabilecek herhangi bir hasar, yaralanma veya kayıp için sorumluluk kabul edilmez.

---

## 📄 Lisans

Bu proje [MIT Lisansı](LICENSE) altında yayınlanmıştır.

"Tesla", "Wall Connector" ve ilgili markalar Tesla, Inc.'e aittir. Bu proje Tesla, Inc. ile bağlantılı veya onun tarafından onaylanmış değildir. Detaylar için [NOTICE.md](NOTICE.md).
