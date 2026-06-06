# Süper Lig Maç Sonuçları Analizi (2020-2024)

**Yazar:** Ahmet Emre Şahin  
**Öğrenci No:** 24 LITT 025  
**Ders:** Veri Analizinde Bilgisayar Programlama 2

🔗 **Canlı Rapor:** https://KULLANICI-ADI.github.io/superlig-analizi/

> Yukarıdaki URL'yi GitHub kullanıcı adınla değiştir (örnek: `https://ahmetemresahin.github.io/superlig-analizi/`).

## Hakkında

Bu rapor, Türkiye Süper Ligi'nin 2020-21'den 2023-24'e kadar olan 4 sezonunu inceler. Toplam 1522 maç verisi üzerinden ev sahibi avantajı, gol dağılımları, takım performansları ve mevsimsel desenler analiz edilmiştir.

## İçerik

- Tanımsal istatistikler (`describe`, `value_counts`, `groupby`, korelasyon)
- 8 farklı görselleştirme:
  - Histogram, bar, boxplot, heatmap (matplotlib/seaborn)
  - 2 etkileşimli Plotly grafiği (takım galibiyet oranları + sezonlara göre sonuç dağılımı)
- Veri temizliği (Şubat 2023 depremi sonrası hükmen kararla sonuçlanan maçların ayrıştırılması)
- Bulgular ve sınırlılıklar bölümü

## Veri Kaynağı

football-data.co.uk verilerinin GitHub yedeği:  
https://github.com/footballcsv/cache.footballdata

## Yerel Çalıştırma

```bash
pip install -r requirements.txt
jupyter notebook notebook/rapor.ipynb
```

## Klasör Yapısı

```
superlig-analizi/
├── data/
│   ├── superlig_2020_2024.csv     # birleşik veri
│   └── tr_*.csv                    # ham sezon dosyaları
├── notebook/
│   └── rapor.ipynb
├── docs/
│   └── index.html                  # GitHub Pages bunu yayınlar
├── requirements.txt
├── .gitignore
└── README.md
```
