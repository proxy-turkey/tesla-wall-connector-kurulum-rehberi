# ⚡ Proje Özeti: Tesla Wall Connector Premium Kurulumu (`summary.md`)

Bu döküman, kırsal bir lokasyonda gerçekleştirilecek olan, her türlü altyapı riskinden izole edilmiş ve tamamen Tesla Wall Connector'a özel olarak tasarlanmış **Premium Güvenlikli Şarj İstasyonu** projesinin özetidir.

---

## 📋 Proje Künyesi

* **Araç:** Tesla EV (Trifaze 16A OBC — 11 kW AC şarj)
* **Lokasyon:** Açık Arazi / Sundurma Altı — WiFi Altyapısı Yok
* **Şarj Gücü:** 11 kW AC sürekli güç (Üç Faz / Trifaze 400V L-L, Faz başına 16A akım)
* **Kurulum Standardı:** Ağır Sanayi ve Veri Merkezi (Data Center) Seviyesi Bağımsız Güvenlik Mimarisi

---

## 📐 Elektriksel Mimari ve Güç Akışı

Sistem, ana binanın mevcut iç tesisatından ve kaçak akım rölelerinden tamamen izole, bağımsız bir otoban olarak kurgulanmıştır. Güç akışı dikey hiyerarşide şu şekildedir:

```
[Ana Ev Panosu: Giriş Barası]
         │
         ▼
[QF1: Siemens 4P 50A C MCB] (Ana Pano İçi Koruma)
         │
         ▼  ➔ (5 Metre 5×6mm² NYY Kablo — Ø25mm Çelik Spiral İçinde)
         │
[Lokal WC Panosu]
         │
    ┌────┴────┐
    │         │
    ▼         ▼
[QF2: 4P 40A C MCB]    [SPD1: Citel 100kA Parafudr — Paralel]
    │
    ▼
[FI1: 4P 63A 30mA Tip A RCD]
    │
    ▼
[KM1: 4P 40A Kontaktör] ◄─── (K1: ENTES GKRC-02F Voltaj Kontrolü)
    │                         │
    ▼                         ▼
[Tesla WC Gen 3] ➔ [Araç]   [F1: 1P 2A Kumanda Sigortası]
```

**Hiyerarşi Notu:** Ev ana panosundaki **QF1 (50A)** sigortası yalnızca otoparka giden 5m besleme hattını korur; lokal panodaki **QF2 (40A)** MCB ise Wall Connector devresinin son ve yerel koruma elemanıdır. Bir arıza durumunda önce QF2 atar — ana panoya yürümek gerekmez.

---

## 🛡️ Premium Koruma ve Altyapı Özellikleri

* **Blackout (Kararma) Engelleme:** Şarj hattı, ana panodaki mevcut kaçak akım rölesinin öncesinden beslenir. Araç şarj olurken yaşanacak anlık dalgalanmalar tesisteki diğer yükleri (güvenlik kameraları, aydınlatma vb.) karanlıkta bırakmaz.

* **Selektivite (Seçicilik) Konforu:** Hattın başına **50A (QF1)**, otopark panosuna **40A (QF2)** sigorta konularak kademeli koruma sağlanmıştır. Bir sorun anında sadece otopark şalteri atar, ana panoya kadar yürümek gerekmez.

* **Sıfırdan Bağımsız TT Topraklama (Bağımsız Lokal TT Sistemi):** Bu sistem, Wall Connector beslemesi için bağımsız lokal TT sistemi olarak tasarlanmıştır. Çiftliğin eski topraklama hattına güvenilmeyerek; `3× Q20 1.5m` bakır çubuk, `25mm²` örgülü bakır ve `bentonit` ile **<10Ω hedefli** (premium: <5Ω) bağımsız bir üçgen topraklama ağı kurulmuştur. Lokal koruma topraklaması yalnızca bu sisteme ait topraklama elektrodu üzerinden sağlanır; ana panodan gelen PE iletkeni bu lokal TT sistemine dahil edilmez. Bu tasarımın amacı, koruma topraklamasını lokal referansa dayandırmak ve farklı topraklama sistemleri arasında koruma iletkeni üzerinden potansiyel taşınmasını (exported potential) önlemektir. Tesla uygulamasında *Ground Monitor* özelliği **ilk kurulumda ENABLED (AÇIK) başlatılacaktır**. Kırsal şebeke dalgalanmalarında 2 kırmızı LED veya RCD trip problemi yaşanırsa son çare olarak Disabled yapılmalıdır.

* **Akıllı Voltaj Filtresi:** **K1: ENTES GKRC-02F** rölesi şebekeyi anlık izler. Voltaj krize girdiğinde (**Düşük Gerilim: 207V, Aşırı Gerilim: 253V** — nominal ±%10) gücü saniyede keser, şebeke düzeldiğinde **25 saniye** bekleyip şarja otomatik devam ettirir.

* **Fiziksel Zırh:** Tüm pano içi köprülerde `6mm² NYAF Pano İçi Güç Köprüleri` (4 farklı renk × 3'er metre olmak üzere toplam **12 metre**) kablo envanteri kullanılarak nizam sağlanmıştır. Beton duvara sıva üstü montajda **Tesla WC wirebox gövdesi için 6mm beton dübel (2 adet — Tesla kutu içeriğinde 2 adet vida ve karton montaj şablonu mevcuttur), Çetinkaya Metal Pano gövdesi için ise 8mm veya 10mm Ağır Hizmet Roket/Çelik Dübel (4 adet)** kullanılacaktır. Spiral boru ve kabloların duvara sabitlenmesinde `Beton Çivili Çelik Kroşe (15 Adet)` kullanılarak mekanik ömür maksimize edilmiştir.

---

## 🔧 Mühendislik Tasarım Değerlendirmeleri

* **ENTES L1-L2-L3 Ortak Köprüleme (Faz Kaybı Körlüğü):** ENTES gerilim algılama uçları F1 sigorta çıkışından (L1) ortak köprülenmiştir. Bu konfigürasyonda aşırı/düşük gerilim L1 üzerinden kusursuz izlenirken; L2 veya L3 fazlarında yaşanabilecek olası bir faz kaybı (phase loss) ENTES tarafından algılanamaz. Bu durum müstakil şarj hattımız için bilinçli bir tasarım tercihidir — **ENTES'in kör noktasını Tesla WC'nin kendi onboard voltaj/faz/frekans denetim işlemcisi kapatır.** Tesla, giriş terminallerinde L2 veya L3 kaybını anında algılar, şarjı bloke eder ve 6 kırmızı flaş hatası basar. Ekstra 3 kutuplu şaltere para vermeye gerek yoktur.

* **50A Sigorta + 6mm² NYY Aşırı Yük Notu:** 6mm² NYY kablonun boru içindeki akım taşıma kapasitesi sınırda olduğundan, 50A sigorta kabloyu aşırı yük (overload) bölgesinde tam koruyamaz, ancak kısa devrelere karşı milisaniyede tam koruma sağlar. **Sahada aşırı yük olasılığı son derece düşüktür:** Hat sadece Tesla WC'ye ait müstakil bir otobandır. Aracın OBC'si donanımsal olarak trifazede 16A'e kilitlidir ve hatta başka hiçbir yük bağlanmaz. Hat ya 16A çekecek ya da kısa devrede sigorta anında kesecektir — kablonun erime senaryosu pratik olarak mümkün değildir.

* **C ve C Eğrisi Selektivite Şerhi:** 50A (C eğrisi) ve 40A (C eğrisi) kesiciler arasında tam selektivite yüksek kısa devre akımlarında garanti edilemeyebilir. Arıza durumunda her iki sigortanın da aynı anda açabileceği sahada bilinmelidir. **Bu bir güvenlik riski değil, sadece konfor meselesidir** — en kötü senaryoda şarj durur, ana panoya yürüyüp şalteri geri kaldırırsınız. Sisteme veya araca zerre zararı yoktur.

* **KM1: 4P Kontaktör Nötr Notu:** Siemens 5TT5840-0 4NO kontaktör AC-1 çalışma sınıfına uygun olup, EVSE sürekli elektrikli araç şarj yükleri için özel olarak seçilmiştir. 4 Kutuplu kontaktör kullanımı TT sistemde nötr hattından gelebilecek harmonik ve sızıntılara karşı **premium bir lükstür** — araç şarj olmuyorken (uykudayken) nötrü kökten ayırmak, aracı kırsal şebekenin tüm elektriksel gürültüsünden korur. Milyonda bir ihtimal olan nötr kontağı temassızlığı (floating neutral) riskine karşı: tüm kontaktör ve şalt vidaları kendi üretici tork değerlerinde (Siemens/ENTES tipik 2.5–3.0 Nm) sıkılmalı, kablo yüksüklerinin tam oturduğundan emin olunmalıdır.

* **RCD Mühendislik Notu:** Tesla WC içerisinde dahili Tip A + DC 6mA kaçak akım algılama sistemi (RCD-DD) bulunduğundan, harici panoda Tip B RCD kullanılmasına gerek yoktur; mevcut Siemens Tip A 30mA FI1 rölesi regülasyonlara tam uyumludur.

---

## 🏷️ Endüstriyel Cihaz Etiketleme Kodları

| Kod | Cihaz | Marka/Model |
|-----|-------|-------------|
| **QF1** | Ana Pano Sigortası (50A MCB) | Siemens 5SL6650-7YA |
| **QF2** | Lokal Pano Şalteri (40A MCB) | Siemens 5SL6640-7YA |
| **FI1** | Kaçak Akım Rölesi (RCD 30mA) | Siemens 5SV3346-6 |
| **KM1** | Güç Kontaktörü (40A, AC-1) | Siemens 5TT5840-0 |
| **SPD1** | Aşırı Gerilim Koruyucu (Parafudr) | Citel DS104RS-230/G/TR |
| **K1** | Gerilim Koruma Rölesi | ENTES GKRC-02F |
| **F1** | Kumanda Sigortası (2A) | Siemens 5SL6102-7 |

---

## 🧰 Ana Bileşen Listesi

| # | Bileşen Kategorisi | Marka / Model / Özellik | Kod |
| --- | --- | --- | --- |
| 1 | **Ana Koruma** | Siemens 5SL6650-7YA (4P, 50A, C Sınıfı MCB) — Ana Pano İçi | QF1 |
| 2 | **Lokal Şalter** | Siemens 5SL6640-7YA (4P, 40A, C Sınıfı MCB) — WC Panosu | QF2 |
| 3 | **Kaçak Akım** | Siemens 5SV3346-6 (4P, 63A, 30mA, Tip A) | FI1 |
| 4 | **Parafudr** | Citel DS104RS-230/G/TR 100kA 4P (Tip I+II+III B+C+D) | SPD1 |
| 5 | **Kontrol Rölesi** | ENTES GKRC-02F Gerilim Koruma Rölesi | K1 |
| 6 | **Güç Kontaktörü** | Siemens 5TT5840-0 (4NO, 40A, 230V AC Bobin, AC-1 sınıfı) | KM1 |
| 7 | **Ana Kablo** | 5×6mm² NYY Besleme Kablosu (Kiriş / Tavan Hattı) | — |
| 8 | **Pano Altyapısı** | Çetinkaya CP 5107 ABS Dağıtım Panosu (Opak Kapaklı, IP65, 3 Sıra x 15 Modül = 45 Otomat Kapasiteli, 35×50×19.5 cm, RAL 7030 Gri) | — |
| 9 | **Topraklama** | Q20 mm × 1.5 m Çubuk (3x) + 25mm² Örgülü Bakır (12m) + Bentonit (10kg) | — |
| 10 | **Kumanda Sigortası** | Siemens 5SL6102-7 (1P, 2A, C Sınıfı MCB) | F1 |
| 11 | **Pano İçi Köprü** | 6mm² NYAF (Kahve/Siyah/Gri/Mavi — 4 renk × 3'er metre) | — |
| 12 | **Kumanda Kablosu** | 1.5mm² NYAF | — |
| 13 | **Nötr + Toprak Barası** | DIN Ray, en az 6 delikli (2 adet) | — |
| 14 | **Yüksük** | İzoleli yüksük 6mm² + ikiz yüksük, 1.5mm² yüksük | — |
| 15 | **Rakor** | PG21 Rakor (pano giriş + WC bağlantısı) | — |
| 16 | **Spiral Boru** | Çelik Spiral Boru Ø25mm — 3 parça: 5m + 0.5m + ~4.5m | — |
| 17 | **Beton Dübel — WC** | 6mm Beton Dübel (Tesla WC wirebox — 2 adet) | — |
| 18 | **Beton Dübel — Pano** | 8mm/10mm Ağır Hizmet Çelik Dübel (Pano — 4 adet) | — |
| 19 | **Kroşe** | Beton Çivili Çelik Kroşe (15 adet) | — |
| 20 | **Aksesuar** | Topraklama klemensi, test klemensi, uyarı etiketi, kablo bağı, ısı shrink | — |

---

## 📱 İşletme ve Bakım Notları

* **📱 Kırsal Altyapı Notu (İnternetsiz İşletme):** Lokal WiFi altyapısı bulunmadığından Tesla WC güncellemeleri otomatik olarak alınamayacaktır. **Periyodik olarak (6 ayda bir)** akıllı telefonunuzu Tesla WC'nin kendi SSID yayınına bağlayıp Tesla One App ➔ Software Update menüsü üzerinden manuel firmware güncelleme kontrolü yapmanız önemle tavsiye edilir.

* **🔔 RCD Periyodik Test Hatırlatması:** FI1 Siemens 5SV3346-6 Tip A Kaçak Akım Rölesi üzerindeki **'T' (Test) butonuna** basılarak **ayda bir kez** periyodik mekanik açma testi gerçekleştirilmeli, rölenin hattı başarıyla kestiği gözle doğrulanmalıdır.

* **🔧 1. Ay Tork Bakımı:** Bakır iletkenlerin zamanla oturma (settling) eğilimi nedeniyle, **ilk enerji verilip sistem 1 ay çalıştırıldıktan sonra** tüm güç terminalleri kontrol edilmelidir: **Wirebox vidaları 5.6 Nm, QF2/FI1/KM1 gibi şalt cihazları üretici katalog torkunda (tipik 2.5–3.0 Nm)** yeniden sıkılmalıdır.

* **🔍 Pano Kapağı Uyarısı (Opak Tasarım):** Panonun kapağı IP65 koruma standartlarında opak (mat gri) tasarıma sahip olduğundan, K1 ENTES ekranındaki anlık şebeke voltaj değerlerini gözlemlemek için pano ön kapağının manuel olarak açılması gerekmektedir.

---

> **📌 Mühendislik Değerlendirmesi:** Bu kurulum mimarisi; voltaj dalgalanmalarına, yıldırım piklerine ve şebeke sızıntılarına karşı Wall Connector'ı ve şarj edilen aracı izole eden, sıfır tavizli, tam kapsamlı bir endüstriyel mimaridir.

---

> **⚠️ ENERJİ VERİLMEDEN ÖNCE SON KONTROL DİREKTİFİ:** TÜM GÜÇ TERMİNALLERİ UYGUN TORK DEĞERLERİNDE (WIREBOX: 5.6 NM, ŞALT CİHAZLARI: ÜRETİCİ KATALOĞU 2.5–3.0 NM) SIKILACAK, İZOLASYON VE SÜREKLİLİK KONTROLLERİ TAMAMLANACAK, ARDINDAN İLK ENERJİ VERİLECEKTİR. İLK 30 DAKİKA TAM YÜKTE ŞARJ ESNASINDA TÜM TERMİNALLER VE KABLOLAR TEMASSIZ KIZILÖTESİ (IR) TERMOMETRE/LAZER ISI ÖLÇER TABANCA İLE TARANMALI; 70°C VE ÜZERİNİ GÖREN KLEMENS VİDALARI YENİDEN TORKLANMALIDIR.
