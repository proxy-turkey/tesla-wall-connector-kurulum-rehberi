# ⚡ Tesla Wall Connector Kurulum Rehberi

Türkiye'de **Tesla Wall Connector Gen 3** (Üç Faz / Trifaze 400V, 11 kW) kurulumu için hazırlanmış, açık kaynaklı ve tam kapsamlı bir rehber. Bu proje; Tesla WC kurmak isteyen, hangi malzemeleri alması gerektiğini ve nasıl kurulacağını arayan kişilere faydalı olması amacıyla yayınlanmıştır.

## 📋 İçindekiler

| Dosya | Açıklama |
|-------|----------|
| [`tesla-wc-kurulum-rehberi.html`](tesla-wc-kurulum-rehberi.html) | İnteraktif HTML rehber — malzeme listesi, SVG diyagram, adım adım kurulum, devreye alma ve uyarılar |
| [`summary.md`](summary.md) | Proje özeti — elektriksel mimari, güç akışı, koruma mimarisi ve mühendislik değerlendirmeleri |
| [`Tesla Wall Connector Alınan Malzemeler - Sayfa1.csv`](Tesla%20Wall%20Connector%20Alınan%20Malzemeler%20-%20Sayfa1.csv) | Tam malzeme listesi (CSV formatında, kategorize edilmiş) |
| [`g3_wc_install_ausnz.md`](g3_wc_install_ausnz.md) | Tesla'nın resmi Wall Connector Gen 3 kurulum kılavuzu (AUS/NZ sürümü, referans amaçlı) |

## 🔧 Sistem Mimarisi

Bu rehber, aşağıdaki mimariyi tarif eder:

- **Güç:** 11 kW AC (Üç Faz 400V L-L, faz başına 16A)
- **Bağımsız Lokal TT Topraklama:** Q20 bakır çubuklar + bentonit ile <10Ω hedefli
- **Kademeli Koruma (Selektivite):** 50A ana pano → 40A lokal pano
- **Gerilim Koruması:** ENTES GKRC-02F (207V/253V eşikler, 25s gecikmeli geri dönüş)
- **Parafudr:** Citel DS104RS-230/G/TR 100kA (Tip I+II+III)
- **Kontaktör:** Siemens 5TT5840-0 (4P 40A, AC-1 sınıfı)
- **Kaçak Akım:** Siemens 5SV3346-6 (4P 63A 30mA Tip A) + Tesla WC dahili RCD-DD

## ⚠️ Önemli Uyarı

> **Bu rehber yalnızca bilgi paylaşımı amacıyla hazırlanmıştır.** Elektrik tesisatı, özellikle de EV şarj sistemleri, **lisanslı bir elektrikçi** tarafından yapılmalıdır. Bu dökümanlardaki bilgiler hiçbir koşulta profesyonel mühendislik danışmanlığının yerine geçmez. Bu projeyi kullanarak oluşabilecek herhangi bir hasar veya yaralanma için sorumluluk kabul edilmez.

## 🌐 HTML Rehberi Görüntüleme

`tesla-wc-kurulum-rehberi.html` dosyasını tarayıcınızda açmanız yeterlidir — harici bağımlılık gerektirmez.

## 📄 Lisans

Bu proje [MIT Lisansı](LICENSE) altında yayınlanmıştır. Tesla Wall Connector kurulum kılavuzu (`g3_wc_install_ausnz.md`) Tesla Inc.'e aittir ve yalnızca referans amaçlı dahil edilmiştir.
